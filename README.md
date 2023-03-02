[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/Celeste1221/ColorStyleTransfer)


# ColorStyleTransfer
This program is modified from a tensorflow tutorial (see code file for link) that uses a deep learning, generative style transfer neural network to transfer the 
style of one image to the content of another. The network is also pre-trained to perform image classification using the VGG19 network architecture. In order to 
accomplish the style transfer, the network uses the intermediate layers of the VGG16 network to separate the style features and the content features of each image so the style of one image can be transferred to the target image, while retaining the original content of the target image. 
Tensorflow is the machine learning platform used. The Python Pillow, scikit-image, NumPy, and Matplotlib libraries are used for image processing, and visualization, and analysis. 

## Dependencies 
```
%pip install --upgrade imageio
%pip install --upgrade scikit-image
%pip install ipywidgets
```
```
import os
import tensorflow as tf
import IPython.display as display
import matplotlib.pyplot as plt
import matplotlib as mpl
import numpy as np
import PIL.Image
import time
import functools
```

## Usage
See ipynb file for input and output images.

## Useful links  
"A Neural Algorithm of Artistic Style" by Leon A. Gatys, Alexander S. Ecker, Matthias Bethge https://arxiv.org/abs/1508.06576



