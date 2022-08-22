# What is Convolutional Neural Network
* CNN is used for image classification, object detection

![](https://preview.ibb.co/nRkBpp/gec2.jpg)

* We have some image ad feature detector(3,3)
* Feature detector can be 3 by 3, 5 by 5 or 7 by 7.
* Feature detector = kernel = filter
* Feauture detector detects features like edges or convex shapes
* Feature map = conv(input image, feature detector). Element wise multiplication of matrices.
* feature map = convolved feature
* Stride = navigating in input image.
* We reduce the size of image. This is important bc code runs faster. However, we lost information.
* We create multiple feature maps bc we use multiple feature detectors(filters).
* Lets look at gimp. Edge detect: [0,10,0],[10,-4,10],[0,10,0]

![](https://image.ibb.co/m4FQC9/gec.jpg)

* After having convolution layer we use ReLU to break up linearity. Increase nonlinearity. Because images are non linear.

![](https://preview.ibb.co/gbcQvU/RELU.jpg)

## What is Same PAdding
* As we keep applying conv layers, the size of the volume will decrease faster than we would like. In the early layers of our network, we want to preserve as much information about the original input volume so that we can extract those low level features.
* input size and output size are same.

![](https://preview.ibb.co/noH5Up/padding.jpg)

## What is Max Pooling
* It makes down-sampling or sub-sampling (Reduces the number of parameters)
* It makes the detection of features invariant to scale or orientation changes.
* It reduce the amount of parameters and computation in the network, and hence to also control overfitting.
## What is Flattening 

![](https://image.ibb.co/c7eVvU/flattenigng.jpg)

## Full Connection
* Neurons in a fully connected layer have connections to all activations in the previous layer
* Artificial Neural Network

![](https://preview.ibb.co/evzsAU/fullyc.jpg)
# Anconda environmet

## Create CNN environment 

* conda create - n CNNenv python=3.9.12

## activate environment
 
* conda activate CNNenv

## İnstall library

* conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
* pip install tensorflow==2.9.1
* pip install keras==2.9.0
* pip install seaborn==0.11.2
* pip install numpy==1.23.1
* pip install pandas==1.4.3 
* pip install matplotlib
* pip install sklearn
	
