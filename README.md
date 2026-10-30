# resnet
Residual connections and trained on CIFAR-10 dataset


Residual CNN for CIFAR-10

A PyTorch implementation of a residual convolutional neural network (ResNet) for image classification on the CIFAR-10 dataset.

## Overview

This project explores how residual connections improve feature learning in convolutional neural networks. The model uses convolutional layers, batch normalization, ReLU activations, shortcut connections, and global average pooling to classify images into 10 categories.

## Dataset

[CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html) contains 60,000 colour images of size 32 × 32 across 10 classes.

- **Training:** 45,000 images
- **Validation:** 5,000 images
- **Testing:** 10,000 images, reserved for final evaluation

## Model Architecture

- Convolutional feature extraction
- Residual blocks with shortcut connections
- Batch normalization and ReLU activation
- Global average pooling
- Fully connected classification layer

Residual learning allows a block to learn a transformation relative to its input:

$$
y = F(x) + x
$$

Projection shortcuts are used when feature dimensions differ.

## Results

After 10 training epochs:

| Metric | Result |
|---|---:|
| Training accuracy | 85.67% |
| Validation accuracy | 77.86% |
| Best validation loss | 0.6633 |

*Test-set performance has not yet been reported.*

## Tech Stack

- Python
- PyTorch
- NumPy
- Matplotlib
- Torchvision
- Scikit-learn

## Future Work

- Evaluate on the untouched test set.
- Implement Grad-CAM visualizations.
- Build an interactive Streamlit application.
- Extend the project to object detection.

## Purpose

This project is part of my practical exploration of deep learning, computer vision, model evaluation, and deployment.
