# ColorStyleTransfer
This program is modified from a tensorflow tutorial (see code file for link) that uses a deep learning, generative style transfer neural network to transfer the 
style of one image to the content of another. The network is also derived from the the intermediate layers of the pre-trained VGG19 image classification network architecture. The network uses the intermediate layers of the VGG16 network to separate the style features and the content features of each image so the style of one image can be transferred to the target image, while retaining the original content of the target image. 
Tensorflow is the machine learning platform used. The Python Pillow, scikit-image, NumPy, and Matplotlib libraries are used for image processing visualization, and analysis. 

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
Initial input images, the first is the content image, the second is the style image, containing the style to be applied to the content image.
Maintaining the color scheme of the content image:
![image](https://user-images.githubusercontent.com/35713658/222324249-ae51fc48-16bc-43e9-b4f8-de4f71015bcd.png)    

Using the color scheme of the style image:  
![image](https://user-images.githubusercontent.com/35713658/222325046-cc2c43e1-3ab7-4a0c-adfb-cafcf105305c.png)

See ipynb file output images.

## Useful links  
"A Neural Algorithm of Artistic Style" by Leon A. Gatys, Alexander S. Ecker, Matthias Bethge https://arxiv.org/abs/1508.06576



