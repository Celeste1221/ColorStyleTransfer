## ColorStyleTransfer
This program is modified from this [tensorflow tutorial](https://www.tensorflow.org/tutorials/generative/style_transfer) that uses a generative style-transfer neural network derived from the the intermediate layers of the pre-trained VGG19 image classification network architecture to separate style and content features of the images in order to transfer the style of one to the content of the other. It uses widgets to ask for user's content and style images. It can keep the original color scheme or apply the color scheme of the style image. 
Tensorflow is the machine learning platform used. The Python Pillow, scikit-image, NumPy, and Matplotlib libraries are used for image processing, visualization, and analysis. 

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

## Output  
Using the color scheme of the style image:  
![image](https://user-images.githubusercontent.com/35713658/222325046-cc2c43e1-3ab7-4a0c-adfb-cafcf105305c.png)     
![image](https://github.com/Celeste1221/ColorStyleTransfer/assets/35713658/623cb365-82b8-4e10-8a64-7e01a1676795)
![image](https://github.com/Celeste1221/ColorStyleTransfer/assets/35713658/adcbe014-8a36-416c-8dbc-02023a0eec2b)



See CF_13_1_ColorStyleTransfer.ipynb file for output images.

## Useful links  
"A Neural Algorithm of Artistic Style" by Leon A. Gatys, Alexander S. Ecker, Matthias Bethge https://arxiv.org/abs/1508.06576



