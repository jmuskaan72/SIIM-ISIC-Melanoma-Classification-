# Context

SIIM-ISIC Melanoma Classification 96

# Content

SIIM-ISIC Melanoma Classification small 96 resized images in .npy format
* x_train_96.npy
* x_test_96.npy

# Acknowledgements

SIIM-ISIC Melanoma Classification to the original Kaggle Competition dataset

# Inspiration

Due to large data set size we have,You will need a lot of images (possibly >10,000) to perform deep learning, and loading those images can take a long time (possibly >1 min). Particularly when you want to make changes to your model over and over, image loading time cannot be negligible. Here, I will introduce how to convert images to a .npy file which will not only reduce the loading time but also memory space and data transfer time when you want to copy the image data to somewhere else. So I convert them into .npy files for faster loading of data and uses size 96 x 96 for loading train and test images. I therefore used  x_train_96.npy file to train my data for better results.
