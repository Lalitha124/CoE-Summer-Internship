#Medical Image Enhancement with Autoencoder
This repository contains a Python project that uses autoencoder models to enhance medical images. The project includes different versions of enhanced autoencoder architectures with techniques like residual connections and SSIM-based loss functions to improve model performance on image quality.

##Project Overview
The main goal is to improve medical images' contrast, sharpness, and overall quality using convolutional neural networks (CNNs) and autoencoder architectures. This project includes models with different configurations and optimizations, such as:

Enhanced Autoencoder with additional convolutional layers
SSIM (Structural Similarity Index) based loss function for improved image quality
Residual and Batch Normalization layers for deeper models
Optimizations with EarlyStopping and ReduceLROnPlateau to manage learning rates

##Requirements
Python 3.x
TensorFlow, Keras, OpenCV, NumPy, Matplotlib, Streamlit

##Data Preparation
Images are stored in .npy format for efficient loading and use.
Data is split into training and testing sets using train_test_split.
Image preprocessing includes resizing to (128, 128) and normalizing pixel values.

##Model Architectures
1.Enhanced Autoencoder v1
This model uses basic CNN layers with SSIM loss to improve the structural quality of the images.

2.Enhanced Autoencoder v2
A more complex model with additional convolutional layers and Batch Normalization for better gradient flow.

3.Enhanced Autoencoder v3
This model adds residual blocks to enhance learning capacity while preventing gradient issues in deep networks.

4. Enhanced Autoencoder v4
Further optimization with additional residual connections and LeakyReLU activation for improved image details.

##Training and Evaluation
Each model is trained with:

SSIM-based loss function
Optional PSNR (Peak Signal-to-Noise Ratio) for evaluating image quality
EarlyStopping and ReduceLROnPlateau callbacks to improve training efficiency

##Deployment with Streamlit
A web application using Streamlit to interact with the model and display image enhancements. To start the app, run:
