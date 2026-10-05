# Toy Neural Network From Scratch

A small neural network implemented from scratch using **NumPy**, without using a deep-learning framework.

## What I built

The network takes 2 input features and predicts one of 3 classes.

2 input features
       ↓
3 hidden neurons (ReLU)
       ↓
3 output neurons (Softmax)

The network includes:

* Forward propagation
* ReLU activation
* Softmax
* Cross-entropy loss
* Backpropagation
* Gradient descent
* Prediction on unseen points
* Decision-region visualization

## Dataset

The toy dataset contains 9 training examples with 2 features and 3 classes.

The three classes form separate clusters:

* Class 0 — bottom-left
* Class 1 — top-right
* Class 2 — top-left

## Training

The network was trained using gradient descent. During training, the loss decreased as the weights were updated using gradients calculated through backpropagation.

## Testing

The trained network correctly classified all 9 training examples and the additional manually selected unseen points tested during development.

I also tested random points and visualized the learned decision regions to examine how the network behaves outside the training examples.

These random points were not assigned ground-truth labels, so they were used to inspect the model's predictions and confidence rather than to calculate test accuracy.

## Why I built this

The purpose of this project was to understand the fundamental mechanics of a neural network rather than relying on a high-level deep-learning framework.

In particular, I wanted to understand how **forward propagation, loss, backpropagation, and gradient descent** work together during training.

## Tools

* Python
* NumPy
* Matplotlib
* Jupyter Notebook

## A potential for future developments in the project

* I would make this project better by adding a labelled dataset, which would help me in getting the testing and training accuracy of this model.
* I would also like to make this same project, but use Sigmoid or Tanh functions in it instead of ReLU activation function, to see how much variation and difference i observe in the model's predictions.
