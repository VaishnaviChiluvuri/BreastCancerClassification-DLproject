🩺 Breast Cancer Classification using Hybrid CNN–LSTM Model
📌 Project Overview

Breast cancer is one of the most common and life-threatening diseases among women worldwide. Early and accurate diagnosis plays a crucial role in improving survival rates.
This project implements a Hybrid Deep Learning model combining Convolutional Neural Networks (CNN) and Long Short-Term Memory (LSTM) to classify breast tumors as Malignant or Benign using the Wisconsin Diagnostic Breast Cancer (WDBC) dataset.

The model leverages:

CNN (Conv1D) for automatic feature extraction

LSTM for learning sequential dependencies among features
to achieve high classification accuracy and robustness.

🎯 Objectives

Build an end-to-end deep learning pipeline for breast cancer classification

Apply a CNN–LSTM hybrid architecture on tabular medical data

Achieve high accuracy with strong generalization

Visualize model performance using multiple evaluation metrics

📂 Dataset Information

Dataset: Wisconsin Diagnostic Breast Cancer (WDBC)

Source: UCI Machine Learning Repository (via scikit-learn)

Samples: 569

Features: 30 numerical features (mean, standard error, worst values of cell nuclei characteristics)

Classes:

0 → Malignant

1 → Benign

🧠 Model Architecture

The proposed model is a Hybrid CNN–LSTM network consisting of:

Conv1D layers (VGG-like blocks):

Extract local spatial patterns from the feature sequence

MaxPooling & Dropout:

Reduce dimensionality and prevent overfitting

LSTM layer:

Capture sequential relationships between extracted features

Dense (Sigmoid) layer:

Perform binary classification

This architecture allows the model to learn both spatial and sequential feature representations.

⚙️ Data Preprocessing

Feature scaling using StandardScaler

Stratified train-test split (80:20)

Reshaping data into 3D format for CNN–LSTM compatibility
(samples, timesteps, features)

📈 Training Configuration

Optimizer: Adam

Loss Function: Binary Cross-Entropy

Batch Size: 32

Epochs: 50

Activation Functions: ReLU (hidden layers), Sigmoid (output layer)

📊 Performance Evaluation

The model is evaluated using:

Accuracy

Precision, Recall, F1-Score

Confusion Matrix

ROC Curve & AUC Score

Training vs Validation Accuracy/Loss plots

🔥 Results (Typical)

Accuracy: 97–99%

ROC-AUC: ~0.99

Low false-positive and false-negative rates

📉 Visualizations

Confusion Matrix Heatmap

Accuracy and Loss Curves

ROC Curve

These visualizations help in understanding model learning behavior and classification performance.
