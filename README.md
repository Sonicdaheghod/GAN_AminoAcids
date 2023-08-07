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


## Credits

* Source code from [SPENCER CHURCHILL](https://www.kaggle.com/code/splcher/starter-anime-face-dataset)
* Amino acid images from wikipedia
