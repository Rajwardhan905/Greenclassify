🌱 GreenClassify
Deep Learning-Based Vegetable Image Classification System

GreenClassify is an end-to-end deep learning web application that classifies vegetable images into 15 predefined categories using a Convolutional Neural Network (CNN). The trained model is deployed using Flask, allowing users to upload images and receive real-time predictions with confidence scores.

📌 Project Overview

This project demonstrates:

Image classification using CNN

Model training and evaluation

Prevention of overfitting using EarlyStopping

Deployment of trained model using Flask

Frontend integration using HTML, CSS, and JavaScript

The system achieves 92.9% test accuracy.

🧠 Problem Statement

Manual vegetable classification in agriculture and retail environments is time-consuming and error-prone. This project aims to automate vegetable classification using deep learning techniques.

🎯 Objectives

Understand Convolutional Neural Networks (CNNs)

Preprocess image datasets for training

Build and train a multi-class classification model

Deploy the trained model as a web application

Provide real-time predictions with confidence scores

📂 Dataset Information

Dataset: Vegetable Image Dataset (Kaggle)

15 vegetable classes

15,000 training images

3,000 validation images

3,000 test images

Classes:

Bean
Bitter_Gourd
Bottle_Gourd
Brinjal
Broccoli
Cabbage
Capsicum
Carrot
Cauliflower
Cucumber
Papaya
Potato
Pumpkin
Radish
Tomato

⚙️ Data Preprocessing

Images resized to 150x150

Pixel values normalized (rescale = 1/255)

Dataset split into train, validation, and test sets

🏗 Model Architecture

Sequential CNN Model:

Conv2D (32 filters, 3x3, ReLU)

MaxPooling2D

Conv2D (64 filters, 3x3, ReLU)

MaxPooling2D

Flatten

Dense (128, ReLU)

Dropout (0.25)

Dense (128, ReLU)

Dense (15, Softmax)

🏋️ Model Training

Optimizer: Adam

Loss: Categorical Crossentropy

Metric: Accuracy

Batch Size: 32

Max Epochs: 30

EarlyStopping (patience = 5)

Training automatically stopped at epoch 9 to prevent overfitting.

📊 Model Performance
Metric	Value
Training Accuracy	~96%
Validation Accuracy	~93–94%
Test Accuracy	92.9%
🚀 Deployment

The trained model is deployed using Flask.

Features:

Upload vegetable image

Real-time prediction

Confidence score display

Clean UI

Structured file architecture

📦 Model File

Due to GitHub's file size limitation (100MB), the trained model file
vegetable_classification.h5 is hosted externally.

🔗 Download Model Here:
https://drive.google.com/file/d/1RhBmEipvR9Z1Z5zac9OpbuiI8ogxrItb/view?usp=sharing

After downloading, place the model file in the project root directory before running the application.

🖥 Application Flow

User → Upload Image → Flask → CNN Model → Prediction → Display Result