# CIS545-BDA_HW4
Image data compression
1. Scale image data (e.g. minmax, standard)
2. Decompose data use PCA or NMF on scaled data
3. Decompose data use Kmeans on scaled or unscaled data
4. Use SSw to find the elbow(cluster numbers) or VRC to find cluster numbers after Kmeans

First: scale image data (matrix); Second: decomposed scaled or unscaled image data (matrix) use PCA, NMF or Kmeans

_______________________________________

Image data and convolutional neural networks
1. Write convolve function to implement kernels on 2D array image with 1 stride and no padding
2. Use a set of kernels on the 2D array image, and then thresholding image
3. Compute the sum, min, max, std after using each kernel
4. Do the classification (square, or circle) on original image, convolutional image, convolutional image with thresholding, 4-statistical numbers of the image.

First: convolute the image, do the thresholding and compute the statistical numbers; second: use these (cleaned data) to do classification
Results: 1. using original image to do classification has a low score, because the features may not so obvious for computers, there are many noises. 2. using the sum of convolution lead to a low score, because it loss many information. 3. using convolution with thresholding has a high score (decrease noises) 4. using 4-statistical numbers also leads to a high score(make better use of the information)
