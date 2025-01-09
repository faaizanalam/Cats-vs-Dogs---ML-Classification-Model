# Cats-vs-Dogs---ML-Classification-Model

This script implements a deep learning-based Cats vs Dogs Image Classification Model using a Convolutional Neural Network (CNN). Here's an overview:

Key Steps:
Dataset Loading and Preprocessing:

Input and labels are loaded from CSV files.
Data reshaped to match the CNN input requirements (100, 100, 3) (RGB images).
Normalization scales the pixel values to the [0, 1] range.
Class weights are calculated to handle potential class imbalances.
Exploratory Data Analysis:

Basic statistics like class distribution and dataset shapes are printed.
Random images are visualized for sanity checks.
Model Definition:

A sequential CNN model is built with:
Three convolutional layers using ReLU activation.
Max-pooling layers to reduce dimensions.
Dropout layers for regularization.
Dense layers to learn higher-order features.
Sigmoid activation for binary classification.
Regularization and learning rate scheduling are applied to improve generalization.
Training and Early Stopping:

The model is compiled with the Adam optimizer, binary cross-entropy loss, and accuracy metric.
Early stopping halts training if validation loss stops improving for 5 epochs.
Evaluation:

The model is evaluated using accuracy and confusion matrices.
Metrics like classification report and F1-score provide detailed performance analysis.
Prediction:

Predictions are made on random test samples and new images.
Results (Cat/Dog) are displayed based on the prediction probability threshold.
Visualization:

Displays confusion matrix to interpret true positives, false positives, etc.
Allows manual testing with custom images.
Features:
Efficient Training: Utilizes class weights and dropout for better handling of class imbalance and overfitting.
Prediction Flexibility: Accepts test data and external images for inference.
Custom Learning Rate Decay: Dynamically adjusts learning rates during training.

Dataset link: https://drive.google.com/drive/u/0/folders/1dZvL1gi5QLwOGrfdn9XEsi4EnXx535bD
