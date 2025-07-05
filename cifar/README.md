# CIFAR-10 Image Classification with a Custom ResNet

A deep learning project focused on classifying images from the [CIFAR-10 dataset](https://www.cs.toronto.edu/~kriz/cifar.html) using a convolutional neural network (CNN) inspired by the ResNet (Residual Network) architecture. This repository contains the complete implementation built from scratch in PyTorch, including custom residual blocks, advanced data augmentation strategies, and comprehensive training and evaluation routines.

---

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Architecture](#architecture)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Training & Evaluation](#training--evaluation)
- [Visualization](#visualization)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Overview

In this project, our goal was to build a robust deep learning model capable of learning complex features from CIFAR-10 images and generalizing well to unseen data. Inspired by the ResNet architecture, our custom model employs residual blocks with skip connections that help mitigate the vanishing gradient problem and enable the training of deeper networks. The project emphasizes clean code organization, reusable components, and effective visualization of training metrics.

---

## Dataset

The project uses the CIFAR-10 dataset which comprises:
- **60,000** 32x32 color images.
- **10 classes** (e.g., airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck).
- **50,000** training images and **10,000** test images.

Learn more about CIFAR-10 on its [official page](https://www.cs.toronto.edu/~kriz/cifar.html).

---

## Architecture

The backbone of this project is a custom implementation of a deep residual network, featuring:
- **Residual Blocks:** Incorporating skip connections to allow gradient flow.
- **Convolutional Layers:** For feature extraction.
- **Data Augmentation:** Techniques to improve model generalization.
- **Optimized Training Pipeline:** Configurable hyperparameters and loss functions.

The architecture is implemented from scratch using PyTorch to provide flexibility and clarity in understanding deep learning model construction.

---

## Features

- **Custom Residual Blocks:** Manually implemented skip connections for deeper networks.
- **Advanced Data Augmentation:** Enhances training data and improves robustness.
- **Modular Code Structure:** Clean and organized modules for model, training, and evaluation.
- **Visualization Tools:** Monitor training progress with dynamic plotting of metrics.
- **Reproducibility:** Clear instructions for setting up the environment and running experiments.

---

## Installation

Follow these steps to set up the project locally:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/cifar10-custom-resnet.git
   cd cifar10-custom-resnet
