# Medical Image Classification with ResNet-18

## Overview

This project was completed as a **group project for CSE 404: Introduction to Machine Learning**. The goal of the project was to develop a deep learning model for **medical image classification** using PyTorch and transfer learning.

We used a pre-trained **ResNet-18 convolutional neural network (CNN)** and fine-tuned it for our classification task. The project involved preparing and augmenting image data, training and validating the model, experimenting with different training configurations, evaluating model performance, and generating predictions on unseen test data.

## Technologies & Techniques

* Python
* PyTorch
* Torchvision
* ResNet-18
* Convolutional Neural Networks (CNNs)
* Transfer Learning
* Image Classification
* Data Augmentation
* AdamW Optimization
* Learning Rate Scheduling
* Model Training & Validation

## Model

Rather than training a convolutional neural network entirely from scratch, we used **transfer learning with a pre-trained ResNet-18 model**.

The final fully connected layer of ResNet-18 was modified to match the number of classes in our dataset. The model was then trained and fine-tuned using our medical image training data.

Our training configuration included **Cross-Entropy Loss**, the **AdamW optimizer**, and a **StepLR learning-rate scheduler**.

## Data Preprocessing & Augmentation

Images were resized to **224 × 224 pixels** to match the input requirements of ResNet-18.

To improve generalization during training, we experimented with data augmentation techniques including:

* Random horizontal flipping
* Random rotation
* Brightness, contrast, and saturation adjustments
* Image normalization

The training, validation, and test datasets were loaded using PyTorch datasets and data loaders.

## Training & Evaluation

The model was trained using separate training and validation stages. During training, we monitored both **loss and classification accuracy** to evaluate model performance.

As part of our experimentation, we adjusted the training process based on validation performance. This included introducing additional data augmentation and a learning-rate scheduler.

Our experiments improved validation performance, with validation accuracy reaching approximately **78%** during our testing.

After training, the model was used to generate predictions for previously unseen test images.

## What I Gained From This Project

This project gave me hands-on experience working with a modern deep learning workflow using PyTorch. Through the project, I gained experience with:

* Training and fine-tuning neural networks
* Transfer learning
* Convolutional neural networks
* Image preprocessing and augmentation
* Training and validation loops
* Hyperparameter experimentation
* Learning-rate scheduling
* GPU-based model training
* Evaluating model performance
* Generating predictions on unseen data

It also gave me experience collaborating with a team on a larger machine learning project and experimenting with changes to improve model performance.

## Group Project & Attribution

This repository contains work completed as part of a **group project for CSE 404**. I am **not claiming sole authorship of the project or the code contained in this repository**. The project was developed collaboratively by members of the group as part of the course.

This repository is being maintained as a **portfolio and professional reference** to demonstrate my experience with machine learning, deep learning, PyTorch, transfer learning, and collaborative software development to prospective employers.

## Usage Notice

This repository is provided **for portfolio and reference purposes only**.

The code and project materials originate from an academic group project and are **not intended to be copied, redistributed, submitted as coursework, or represented as another individual's work**.

If you are a current or future student completing a similar assignment, please follow your institution's academic integrity policies and do not use this repository as a submission for coursework.
