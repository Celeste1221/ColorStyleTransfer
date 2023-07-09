## ColorStyleTransfer
This program is modified from this [tensorflow tutorial](https://www.tensorflow.org/tutorials/generative/style_transfer) that uses a generative style-transfer neural network derived from the the intermediate layers of the pre-trained VGG19 image classification network architecture to separate style, color scheme, and content features of the images in order to transfer the style of one to the content of the other. It uses widgets to ask for user's content and style images. The user can keep the content image's color scheme or apply the color scheme of the style image. 

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
### Input: 
![image](https://user-images.githubusercontent.com/35713658/222324249-ae51fc48-16bc-43e9-b4f8-de4f71015bcd.png)   
The image of the white husky is the content image. Notre Dame's stained glass window is the style image. This stained glass style will be applied to the husky. The stained glass image looks faded out because the color scheme of the white husky image has been applied to it first. This way, the final output image will look like a stained glass white husky. 
### Output:
![image](https://github.com/Celeste1221/ColorStyleTransfer/assets/35713658/d3ba982d-0235-4465-b725-4fb9ab0dd284)  
10 epochs, 100 steps per epoch
### Input:
![image](https://user-images.githubusercontent.com/35713658/222325046-cc2c43e1-3ab7-4a0c-adfb-cafcf105305c.png)   
Here, the vibrant colors of the stained glass window remain and will be applied to the husky image, so the output image will look like a colorful stained glass husky.
### Output:
![image](https://github.com/Celeste1221/ColorStyleTransfer/assets/35713658/7e2866da-724c-46e9-8f88-99269604ae0b)  
10 epochs, 64 steps per epoch
![image](https://github.com/Celeste1221/ColorStyleTransfer/assets/35713658/adcbe014-8a36-416c-8dbc-02023a0eec2b)  
100 epochs, 64 steps per epoch
## Useful links  
"A Neural Algorithm of Artistic Style" by Leon A. Gatys, Alexander S. Ecker, Matthias Bethge https://arxiv.org/abs/1508.06576



