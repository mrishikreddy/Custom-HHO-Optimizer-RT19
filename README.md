# Breast Cancer Classification with ANN and HHO Optimization

This project implements a binary classification model for breast cancer diagnosis using an Artificial Neural Network (ANN) optimized via the Harris Hawks Optimization (HHO) algorithm. It demonstrates training performance, prediction accuracy, and visualizations of model metrics over epochs.

[Visit Live Project](https://colab.research.google.com/drive/1pildqHmi2xMRkjqmcDswzVgUgu609FzM?usp=sharing)

---

## Table of Contents

- [Installation Instructions](#installation-instructions)  
- [Usage](#usage)  
- [Features](#features)

---

## Installation Instructions

### Prerequisites

- Python 3.x
- Libraries:
  ```bash
  pip install numpy pandas tensorflow scikit-learn matplotlib seaborn
  ```

### Dataset

- CSV file: `cell_data.csv` must be available in your working directory or Colab environment.
- The file should contain attributes for cytology cell features and a classification label.

---

## Usage

1. **Preprocess the Dataset**
   - Handles missing values and encodes labels.
   - Scales features using `StandardScaler`.

2. **Build the ANN Model**
   - Sequential model with ReLU activations and sigmoid output.
   - Designed for binary classification tasks.

3. **Optimize with HHO Algorithm**
   - HHO is used instead of traditional backpropagation.
   - Loss and accuracy are tracked across iterations.

4. **Evaluate the Model**
   - Generates a confusion matrix and test accuracy.
   - Predicts sample input for quick inference.
   - Plots training loss and accuracy curves.

---

## Features

- Binary classification of cell samples (Benign/Malignant).
- Custom implementation of Harris Hawks Optimization (HHO).
- Accuracy and binary cross-entropy loss visualization.
- No use of built-in Keras training APIs – optimization is fully custom.
- Predicts single sample after training completion.
- Loss and accuracy are plotted over epochs to monitor performance.

---

> **Note:** HHO is a metaheuristic optimizer and may take longer to converge than traditional gradient-based methods. Recommended to run in a GPU-enabled environment such as Google Colab.

