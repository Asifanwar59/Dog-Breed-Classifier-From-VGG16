[//]: # (Image References)

## Project Overview

Welcome to the Convolutional Neural Networks (CNN) project in the Artificial Intelligence! This project aims at building a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, the algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed. The code is build using a pre-trained VGG16 network. 

## Project Instructions

### Instructions

1. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`.  The `dogImages/` folder should contain 133 folders, each corresponding to a different dog breed.
2. Download the [human dataset](http://vis-www.cs.umass.edu/lfw/lfw.tgz).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 
3. Make sure you have already installed the necessary Python packages used in the dog_app.ipynb file. refer section "Installations" below. 
4. Open the notebook and follow the instructions.
	
	```
		jupyter notebook dog_app.ipynb
	```

### Installations
__NOTE__ Replace conda with you environment installtion commands

`conda install os openCV matplotlib`
`conda install numpy PIL`
`conda install tqdm torch torchvision`


__NOTE:__ While some code was already been implemented by Udacity team to get me started, I implemented additional functionality to demonstrate a Dog Breed classifier model. The model has two parts, one is develped from scratch and the other one using VGG16 pretrained model.

__NOTE:__ PyTorch is used to train the CNNs.

## (Optionally) Accelerating the Training Process 

If the code is taking too long to run, you will need to switch to running your code on a GPU.  

## Project Specifications:

1. The model returns the percentage of the first 100 images in the dog and human face datasets that include a detected, human face.
2. Use a pre-trained VGG16 Net to find the predicted class for a given image. 
3. The submission returns the percentage of the first 100 images in the dog and human face datasets that include a detected dog.
4. Choose appropriate loss and optimization functions for this classification task. Train the model for a number of epochs and save the "best" result.
5. The trained model developed from pretrained VGG16 model attains accuracy on the test set is 60% or greater.
6. The model tests at least 6 images, including at least two human and two dog images.
