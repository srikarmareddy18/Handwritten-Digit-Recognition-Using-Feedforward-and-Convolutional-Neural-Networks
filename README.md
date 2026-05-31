# Handwritten-Digit-Recognition-Using-Feedforward-and-Convolutional-Neural-Networks
This project compares Feedforward Neural Networks (FNNs) and Convolutional Neural Networks (CNNs) for handwritten digit classification using the MNIST dataset. Both models were trained and evaluated across multiple runs, with CNNs achieving superior accuracy through effective feature extraction and spatial pattern recognition

## Overview

This project implements and compares two neural network architectures for handwritten digit classification using the MNIST dataset:

* Feedforward Neural Network (FNN)
* Convolutional Neural Network (CNN)

The models are built using TensorFlow/Keras and trained on the MNIST dataset.

## Features
* Loads MNIST data from IDX files
* Normalizes image pixel values
* Applies one-hot encoding to labels
* Implements a fully connected neural network
* Implements a convolutional neural network
* Trains and evaluates both models
* Requirements
* Python 3.x
* TensorFlow
* NumPy

## Install dependencies:
pip install tensorflow numpy

##Dataset Files
Place the following files in the project directory:

* train-images-idx3-ubyte (WARNING: This file exceeded GitHub's 25MB size limit, precluding it from this repository so you will have to find it online )
* train-labels-idx1-ubyte
* t10k-images-idx3-ubyte
* t10k-labels-idx1-ubyte

## Usage
Run the script: **python mnist_classification.py** and the program will train both models and display their test accuracies.

## Model Architectures
### FNN
* Flatten
* Dense (256, ReLU)
* Dense (128, ReLU)
* Dense (64, ReLU)
* Dense (10, Softmax)
### CNN
* Conv2D (32 filters, 3×3)
* MaxPooling2D
* Conv2D (64 filters, 3×3)
* MaxPooling2D
* Flatten
* Dense (128, ReLU)
* Dense (64, ReLU)
* Dense (10, Softmax)
