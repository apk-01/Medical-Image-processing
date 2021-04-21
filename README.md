# Medical-Image-processing
This repository explores the various medical image processing techniques using Python. We shall be using modules like: scikit-image, PIL, opencv, flowdec and starFISH.
We are using sample data from https://scikit-image.org/docs/stable/api/skimage.html and https://cellprofiler.org/

The codes are written on : google colaboratory (https://colab.research.google.com/notebooks/intro.ipynb)

# 3D deconvolution
Deconvolution is an image processing technique used to improve the contrast and sharpness of images captured using a light microscope. Each point source below the diffraction limit is blurred by the microscope into what is known as a point spread function (PSF). Deconvolution functions use this known PSF values(based on microcope's parameters) to deblur the images.

Example:


![Deconvolution](/images/BX3-and-Deconvolution.jpg)


# Image segmentation and edge detection

In medical imaging, it is very important to identify the region of interest and extract features from them. There are several ways to do so such as: thresholding, edge detection, segmentation and contouring. These techniques are based on intensity values, and works by either getting the intensity manually from user or automatically finds the difference between background and foreground.

Example:

![Edge detection](/images/Example-of-cell-segmentation-and-tracking-in-the-C-elegans-embryogenesis-image-sequence.png)
