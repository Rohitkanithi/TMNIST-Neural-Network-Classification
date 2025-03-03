# TMNIST Character Recognition - CNN Model

## Overview

This project focuses on **handwritten character recognition** using the **TMNIST (Typography MNIST) dataset**, which contains **94 unique characters** including uppercase/lowercase letters, digits, and symbols. The dataset provides a diverse set of handwritten characters across various typefaces, making it more challenging than traditional MNIST.

We employ a **Convolutional Neural Network (CNN)** for classification, achieving high accuracy by leveraging **data augmentation, batch normalization, dropout regularization, and hyperparameter tuning**.

## Dataset

The dataset used is **TMNIST Alphabet (94 characters)** from Kaggle:

- **Dataset URL:** [TMNIST Alphabet (94 characters)](https://www.kaggle.com/nikbearbrown/tmnist-alphabet-94-characters/)
- **Number of Classes:** 94 (A-Z, a-z, 0-9, symbols)
- **Total Images:** ~281,000
- **Image Size:** 28x28 grayscale

## Methodology

### **1. Data Preprocessing**
- Image resizing and normalization
- One-hot encoding for labels
- Data augmentation (rotation, shifting, zooming)
- Splitting into **training (80%)** and **testing (20%)** sets

### **2. CNN Model Architecture**
- **4 Convolutional Layers** with **Batch Normalization & ReLU Activation**
- **MaxPooling** for downsampling
- **Dropout Regularization** to prevent overfitting
- **Fully Connected Layers** with **Softmax Activation** for classification

### **3. Training & Optimization**
- **Loss Function:** Categorical Crossentropy
- **Optimizer:** Adam
- **Performance Metrics:** Accuracy, Precision, Recall
- **Hyperparameter tuning** for best results
- **Early Stopping** to prevent overfitting

### **4. Evaluation**
- Achieved **92.28% accuracy** on the test set
- Evaluated using **Confusion Matrix** and **Loss/Accuracy plots**
