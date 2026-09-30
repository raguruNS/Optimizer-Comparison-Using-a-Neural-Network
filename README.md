# Project 9: Optimizer Comparison Using a Neural Network

## 📌 Project Overview

This project demonstrates how different optimization algorithms affect the training of a neural network.

A simple neural network is built using the **Iris classification dataset**. Two commonly used optimizers, **Stochastic Gradient Descent (SGD)** and **Adam**, are used to train the neural network.

The training loss, training accuracy, and test classification performance are compared to understand the differences between the two optimization algorithms.

---

## 🎯 Objectives

The main objectives of this project are:

* Build a simple neural network using the Iris dataset.
* Preprocess and standardize the dataset.
* Train the neural network using SGD.
* Train the neural network using Adam.
* Compare training loss between SGD and Adam.
* Compare training accuracy between the optimizers.
* Evaluate the classification performance on the test dataset.
* Understand the role of optimizers in neural network training.

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Matplotlib**
* **Scikit-learn**
* **TensorFlow / Keras**
* **Google Colab / Jupyter Notebook**

---

## 📊 Dataset

The **Iris dataset** is used for this project.

The dataset contains:

* **150 samples**
* **4 input features**
* **3 target classes**

### Input Features

1. Sepal Length
2. Sepal Width
3. Petal Length
4. Petal Width

### Target Classes

1. Setosa
2. Versicolor
3. Virginica

---

## 🧠 Neural Network Architecture

The neural network used in this project contains:

```text
Input Layer
    ↓
4 Features
    ↓
Dense Layer - 16 neurons - ReLU
    ↓
Dense Layer - 8 neurons - ReLU
    ↓
Output Layer - 3 neurons - Softmax
```

The output layer contains three neurons because the Iris dataset has three classification classes.

---

## ⚙️ Optimizers Used

### 1. Stochastic Gradient Descent (SGD)

SGD updates the neural network parameters using gradients of the loss function.

Configuration used:

```text
Learning Rate = 0.01
Batch Size = 16
Epochs = 100
```

### 2. Adam

Adam is an adaptive optimization algorithm that adjusts the learning process using estimates of the gradients and their moments.

Configuration used:

```text
Learning Rate = 0.001
Batch Size = 16
Epochs = 100
```

---

## 🔄 Project Workflow

The project follows these steps:

```text
Load Iris Dataset
       ↓
Preprocess Dataset
       ↓
Train/Test Split
       ↓
Feature Standardization
       ↓
Build Neural Network
       ↓
Train using SGD
       ↓
Train using Adam
       ↓
Compare Training Loss
       ↓
Compare Training Accuracy
       ↓
Evaluate Test Performance
       ↓
Compare Results
```

---

## 📈 Evaluation

The two optimizers are compared using:

* Training Loss
* Training Accuracy
* Test Accuracy
* Classification Report

The loss and accuracy curves are plotted to visualize the training behavior of SGD and Adam.

---

## 📉 Expected Results

The project generates the following outputs:

### Training Loss Graph

A graph comparing the training loss of SGD and Adam over the training epochs.

### Training Accuracy Graph

A graph comparing the training accuracy of SGD and Adam.

### Classification Performance

The test accuracy and classification report for both models are displayed.

The exact accuracy values may vary depending on factors such as initialization, TensorFlow version, and training conditions.

---

## 📂 Project Structure

```text
Project-9-Optimizer-Comparison/
│
├── optimizer_comparison.ipynb
├── README.md
│
└── screenshots/
    ├── iris_dataset.png
    ├── train_test_split.png
    ├── neural_network.png
    ├── sgd_training.png
    ├── adam_training.png
    ├── loss_comparison.png
    ├── accuracy_comparison.png
    ├── sgd_evaluation.png
    ├── adam_evaluation.png
    └── final_comparison.png
```

---

## 💻 How to Run the Project

### Step 1: Open Google Colab or Jupyter Notebook

Open the provided `.ipynb` notebook.

### Step 2: Install TensorFlow if Required

```bash
pip install tensorflow
```

### Step 3: Import the Required Libraries

```python
import numpy as np
import matplotlib.pyplot as plt

from sklearn.datasets import load_iris
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.metrics import accuracy_score, classification_report

from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Dense
from tensorflow.keras.optimizers import SGD, Adam
```

### Step 4: Run the Notebook

Execute the notebook cells in order.

### Step 5: Observe the Results

Check:

* SGD training results
* Adam training results
* Loss comparison graph
* Accuracy comparison graph
* Test accuracy
* Classification reports

---

## 🔍 Analysis

The project demonstrates that the optimizer plays an important role in neural network training.

SGD uses gradient-based updates with a fixed learning rate, while Adam uses an adaptive approach to update the model parameters.

Although both models use the same neural network architecture and dataset, their training behavior can differ. The loss and accuracy graphs provide a visual comparison of how the models learn during training.

The final test accuracy and classification reports provide additional information about the classification performance of each trained model.

---

## ✅ Conclusion

This project successfully demonstrates the comparison of **SGD and Adam optimizers** using a neural network trained on the Iris dataset.

The experiment shows how different optimizers influence the training process, loss reduction, and classification performance.

By comparing the training graphs and final evaluation results, the behavior of the two optimization algorithms can be studied in a practical Machine Learning environment.

---

## 👨‍💻 Project Information

**Project:** Project 9 – Optimizer Comparison Using a Neural Network

**Dataset:** Iris Dataset

**Machine Learning Task:** Multi-Class Classification

**Optimizers:** SGD and Adam

**Programming Language:** Python

**Libraries:** NumPy, Matplotlib, Scikit-learn, TensorFlow/Keras

**Environment:** Google Colab / Jupyter Notebook
