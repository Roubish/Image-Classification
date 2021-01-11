# Image Classification with Pre-trained Keras models
## Introduction

In this project, we will be using resnet50 which was originally trained to classify the imagenet data. We shall use this model to predict the class of an input image. We shall understand the different steps of preprocessing this input image as required by the network, before predicting the class of the image.
## Importing the Modules

Let's begin by importing the necessary modules.
## Getting the Model and Pre-trained Weights

We need to include models and processing packages that are specific to that model.

## Loading the Image
![](lion.jpg)
Let us load the image we want to classify using this model.
## Predicting the Class using Pre-Trained model

Now that we have loaded the image and the pre-trained network, we shall preprocess the image, feed it to the neural network to predict the class of the image.
#### Note::

- image.img_to_array : Converts a PIL Image instance to a Numpy array.

- tensorflow.keras.applications.resnet50.preprocess_input : The images are converted from RGB to BGR, then each color channel is zero-centered with respect to the ImageNet dataset, without scaling.

- tensorflow.keras.applications.resnet50.decode_predictions : Decodes the prediction into a list of tuples (class, description, probability)
