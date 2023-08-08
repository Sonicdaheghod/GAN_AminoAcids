# Generative Adversarial Network (GAN) - Amino Acid Dataset
by Megan Tran

## Table of Contents
* [Purpose of Program](#Purpose-of-program)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Using the Program](#Using-the-Program)
* [Credits](#Credits)

## Purpose of Program

* Practicing building and executing a GAN on my own amino acid dataset.
* Used dataset to generate novel amino acids.

## Screenshots

Real Dataset images (left) vs Fake Generated Images (right)
![image](https://github.com/Sonicdaheghod/GAN_AminoAcids/assets/68253811/8579222e-88e2-49cd-bb8b-6ce607c2a70d)


## Technologies
Languages/ Technologies used:

* Jupyter Notebook

* Kaggle

* Python3
  
## Setup

Download the necessary packages:

```
pip install torch
pip install torchvision
pip install pandas
pip install numpy
pip install matplotlib

```
Check to see if version of Python/Python3 (if on jupyter Notebook) is used, this is to ensure packages work properly. Python 3.8 or better is recommended.

```
import sys
sys.version
```
Import the following libraries:

```

#for model
%matplotlib inline
import argparse
import os
import random
import torch
import torch.nn as nn
import torch.nn.parallel
import torch.backends.cudnn as cudnn
import torch.optim as optim
import torch.utils.data
import torchvision.datasets as dset
import torchvision.transforms as transforms
import torchvision.utils as vutils
import numpy as np

#showing generation of fake images
import matplotlib.pyplot as plt
import matplotlib.animation as animation
from IPython.display import HTML

```
## Using the Program

1) Essential Variables

There are variables defined that are used for preparing the dataset, setting up the GAN model, and displaying the results.

1a) Increased Epochs

I increased the number of epochs to 500 so the model would be better trained to produce fake images that were similar to the real images. Using the original number of epochs lead to fake images that appeared as noise.

```
# Number of training epochs
num_epochs = 500 # Original is 5 on a dataset of 1 million

```

2) DCGAN Implementation
* Weights initialized to prevent vanishing gradient problem.
* Generator was set up for producing fake images that could pass off as real images.
* Discriminator set up for detecting if an image was real or fake.
* Loss function detects differences between real and fake images, optimizer minimizes those differences.
* Dataset is then run through the model using the number of epochs, steps, and learning rate defined in variables.
  
3) Results

* Peformance of both gneerator and discriminator visualized using loss plot. Plot shows stability of both, so generator products images that pass off as "real" and discriminator can distinguish between real and fake image.
![image](https://github.com/Sonicdaheghod/GAN_AminoAcids/assets/68253811/996bdfa7-5a75-4bb8-8bc5-87829a83e46e)

* The loop of the training process was also included in the code. This shows the process of how the model wa learned how to produce amino acids that were siliar to that in the training dataset.
  
* Real images vs fake images are shown for comparison.
<img width="586" alt="image" src="https://github.com/Sonicdaheghod/GAN_AminoAcids/assets/68253811/720c933c-ae98-4250-aa58-7b57e244e6de">




## Credits

* Source code from [SPENCER CHURCHILL](https://www.kaggle.com/code/splcher/starter-anime-face-dataset)
* Amino acid images from wikipedia
