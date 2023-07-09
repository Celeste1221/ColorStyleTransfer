## ColorStyleTransfer
This program is modified from this [tensorflow tutorial](https://www.tensorflow.org/tutorials/generative/style_transfer) that uses a generative style-transfer neural network derived from the the intermediate layers of the pre-trained VGG19 image classification network architecture to separate style, color scheme, and content features of the images in order to transfer the style of one to the content of the other. It uses widgets to ask for user's content and style images. It can keep the original color scheme or apply the color scheme of the style image. 
Tensorflow is the machine learning platform used. Python Pillow, Scikit-Image, NumPy, and Matplotlib are used for image processing, visualization, and analysis. 

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
### Input images: the first image is the content image, the second is the image containing the style that will be applied to the content image. In this first example, the stained glass image (style image) is faded out because the color scheme of the white dog image (content image) has been applied to it first. This way, the final output image should be a stained glass white dog.  
Maintaining the color scheme of the content image:
![image](https://user-images.githubusercontent.com/35713658/222324249-ae51fc48-16bc-43e9-b4f8-de4f71015bcd.png)   
### In this second example, the color scheme as well as the style of the stained glass image has been applied to the white dog picture. In this project, you have the choice.
Using the color scheme of the style image:  
![image](https://user-images.githubusercontent.com/35713658/222325046-cc2c43e1-3ab7-4a0c-adfb-cafcf105305c.png) 

### Output  
![image](https://github.com/Celeste1221/ColorStyleTransfer/assets/35713658/7e2866da-724c-46e9-8f88-99269604ae0b)
![image](https://github.com/Celeste1221/ColorStyleTransfer/assets/35713658/adcbe014-8a36-416c-8dbc-02023a0eec2b)



See CF_13_1_ColorStyleTransfer.ipynb file for output images.

## Useful links  
"A Neural Algorithm of Artistic Style" by Leon A. Gatys, Alexander S. Ecker, Matthias Bethge https://arxiv.org/abs/1508.06576



