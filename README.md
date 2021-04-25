# Medical-Image-processing
This repository explores the various medical image processing techniques using Python. We shall be using modules like: scikit-image, PIL, opencv, flowdec and starFISH.
We are using sample data from https://scikit-image.org/docs/stable/api/skimage.html and https://cellprofiler.org/

The codes are written on : google colaboratory (https://colab.research.google.com/notebooks/intro.ipynb)

**To execute the codes locally:**
1. Set up anaconda
2. Add python 3.6+
3. Remove google colab file uploading cell from the notebook
4. Install the dependencies(imported libraries) before executing the program
5. Execute the code with your own data/images

**To execute with google colab:**
1.Upload your own data/images while executing the upload cell
2.Replace the file reading file names with your image file names
3.Execute the remaining cells 

# 3D deconvolution
Deconvolution is an image processing technique used to improve the contrast and sharpness of images captured using a light microscope. Each point source below the diffraction limit is blurred by the microscope into what is known as a point spread function (PSF). Deconvolution functions use this known PSF values(based on microcope's parameters) to deblur the images.

Example:


![Deconvolution](/images/BX3-and-Deconvolution.jpg)


# Image segmentation and edge detection

In medical imaging, it is very important to identify the region of interest and extract features from them. There are several ways to do so such as: thresholding, edge detection, segmentation and contouring. These techniques are based on intensity values, and works by either getting the intensity manually from user or automatically finds the difference between background and foreground.

Example:

![Edge detection](/images/Example-of-cell-segmentation-and-tracking-in-the-C-elegans-embryogenesis-image-sequence.png)

# Image enhancement

Image Enhancement is an important technique in image processing, used to improve the contrast or quality of images for better display and further analysis. Different methods are used to achieve this, namely, Histogram equalization, log/gamma adjust, intensity rescaling, etc.

Example:


![Enhancement](/images/imageEnhac.png)

# 3D image chunking and stitching

Sometimes medical images, especially 3D images can be very large in size and we might not have enough GPU to process on them. In such cases, we would need to chunk the images into smaller parts and process each chunk individually. We shall then stitch back the processed chunks back together to get the original image shape. This can be achieved very easily through the Python package, Dask.

Example:

![Dask](/images/dask.png)

# Image registration

Image registration is a very important part of medical imaging. We often get images of the same object from different sources or images taken sequentially from the same source. Such images may require to be overlayed for further processing. However, since they have been taken sepperately, they might not be aligned properly. In such a case, we need to align the images appropriately before processing on them. In our notebook we shall explore one of the most popular methods of image registration.

Example:

![Registration](/images/registration.png)
