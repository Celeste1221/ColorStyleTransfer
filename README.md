# ColorStyleTransfer
This program is modified from a tensorflow tutorial (see below) that uses a deep learning, generative style transfer neural network to transfer the 
style of one image to the content of another. The network is also pre-trained to perform image classification using the VGG19 network architecture. In order to 
accomplish the style transfer, the network uses the intermediate layers of the VGG16 network to separate the style features and the content features of each image so that
the style of one image can be transferred to the target image, while retaining the original content of the target image.
The code has been modified so that the user can upload their own style and content images and they can choose to either retain the general coloring of the 
target content image and only apply the style of the style image, or they can apply both the style and the general coloring of the style image to the target image. 
It uses IPyWidgets for users to upload their chosen target image as well as their chosen style image. Tensorflow is the machine learning platform used. The Python Pillow, scikit-image, NumPy, and Matplotlib libraries are 
used for image processing and visualization, and analysis. 

## Dependencies 
'''%pip install --upgrade imageio
%pip install --upgrade scikit-image
%pip install ipywidgets
import os
import tensorflow as tf
import IPython.display as display
import matplotlib.pyplot as plt
import matplotlib as mpl
import numpy as np
import PIL.Image
import time
import functools'''

## Usage
Snippets of code, widgets, and inputs/outputs here

## Useful links  
"A Neural Algorithm of Artistic Style" by Leon A. Gatys, Alexander S. Ecker, Matthias Bethge https://arxiv.org/abs/1508.06576



