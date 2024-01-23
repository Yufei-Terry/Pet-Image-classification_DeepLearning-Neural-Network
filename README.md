# Pet 😸 and 🐶 Image Classification Problem - Neural Network - will be uploaded soon


## Table of Contents
1. Business Understanding (Business Context)
2. Data Preparation and Processing\
   2.1. Import Libraries\
   2.2. Preprocessing\
        2.2.1. Extract and generate image\
        2.2.2. EarlyStopping setting
3. Modeling\
   3.1. Convolutional Network\
   3.2. Convolutional Network with multiple different epoch\
   3.3. Stack model with transfer learning and convolutional network\
   3.4. Transfer learning Xception model
4. Evaluate the model\
   4.1. Generate prediction\
   4.2. Confusion Matrix
5. Conclusion


### 1. Business Understanding (Business Context) 


## 2. Data processing
   ### 2.1. Import Libraries
   ```python
# This Python 3 environment comes with many helpful analytics libraries installed
# It is defined by the kaggle/python Docker image: https://github.com/kaggle/docker-python
# For example, here's several helpful packages to load

import numpy as np # linear algebra
import pandas as pd # data processing, CSV file I/O (e.g. pd.read_csv)

# Input data files are available in the read-only "../input/" directory
# For example, running this (by clicking run or pressing Shift+Enter) will list all files under the input directory

import os
for dirname, _, filenames in os.walk('/kaggle/input'):
    for filename in filenames:
        print(os.path.join(dirname, filename))

# You can write up to 20GB to the current directory (/kaggle/working/) that gets preserved as output when you create a version using "Save & Run All" 
# You can also write temporary files to /kaggle/temp/, but they won't be saved outside of the current session


#package for data preparation
import zipfile
import glob
from random import shuffle
import gc
import cv2
from tqdm import tqdm #can display the progress bar
import matplotlib as plt
import matplotlib.pyplot as plt




  
   ```
