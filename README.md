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
pip install scikit-learn
pip install pandas
pip install numpy
pip install matplotlib
```
Check to see if version of Python/Python3 (if on jupyter Notebook) is used, this is to ensure packages work properly. Python 3.8 or better is recommended.

```
import sys
sys.version
```

Import the following packages and libraries:

```
# Data processing
import pandas as pd
import numpy as np

# Visualizing Dataset
import matplotlib as plt
import matplotlib.pyplot as plt

# Model
from sklearn.model_selection import train_test_split
from sklearn import svm
from sklearn.svm import SVC
```
## Using the Program
1) Data Cleaning and Preprocessing


2) SVM Model


3) Evaluating Model


## Credits

* Source code from [SPENCER CHURCHILL](https://www.kaggle.com/code/splcher/starter-anime-face-dataset)
* Amino acid images from wikipedia
