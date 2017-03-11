# Image Classification of CIFAR-10 dataset

In this project, I classify images from the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) using tensorflow. 
The dataset consists of airplanes, dogs, cats, and other objects. I preprocess the images, then train a convolutional neural network on all the samples. The images are normalized and the labels are one-hot encoded.

### Dataset

##### The dataset is broken into batches.  The CIFAR-10 dataset consists of 5 batches, named `data_batch_1`, `data_batch_2`, etc.. Each batch contains the labels and images that are one of the following:
###### * airplane
###### * automobile
###### * bird
###### * cat
###### * deer
###### * dog
###### * frog
###### * horse
###### * ship
###### * truck

### Architecture

The network has the following layers - 

Input -> Conv -> Max pooling -> Conv -> Max pooling -> Conv -> Max pooling -> FC (1024) > Dropout -> FC(128) -> Dropout -> Output

#####Input (32 x 32 x 3)
#####Conv Layer (depth = 32, stride = 1, padding= "SAME")
#####Max pooling (pool size = 2. pool strides = 2)
#####Dropout (0.75)

### Results

Accuracy on test data = 73%
