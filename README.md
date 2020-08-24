# Attack on Image Classification Network

## This project works in two stage:-
1. Classification of Image from a given dataset using VGG-16.

2. Performing attack on image (Adding some perturbation so that the same Model classify the input incorrectly.)


## Prerequisites
Python, TensorFlow, Foolbox, Download ImageNet dataset.
Use Google Colab for running the project if you don't have high computing power.

## Source:-
https://arxiv.org/pdf/1801.00553.pdf

## Classification Model
We have used pre-trained model VGG16 for classification of image from IMAGENET dataset.

## Attack
1. LBFGS Attack:-
This attack has been performed directly by importing LBFGS attack from foolbox library.

2. Iterative FGSM Attack:-
This attack has been performed by computed gradient iteratively to compute adversarial input.

3. PGD(Projected Gradient Descent) Attack:-
 This attack has been performed by iterative computation of gradient descent in such a way that the difference between given input and adversarial input is always less than epsilon.


