# 🌴 Date Fruit Classification using PyTorch ANN

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

An automated classification system that identifies 7 different varieties of date fruits using morphological features and an **Artificial Neural Network (ANN)**.

---

## 📖 Overview
The quality and variety of date fruits are traditionally determined by human experts. This project automates that process by analyzing **34 distinct features** (including Area, Perimeter, and Color Metadata) extracted from high-resolution images.

### 🎯 Objective
To build a robust deep learning model that classifies dates into one of the following categories:
*Barhee, Deglet Noor, Sukkari, Rotana, Safawi, Ithem, and Sogay.*

---

## 🛠️ Technical Architecture

### 📊 Data Preprocessing
* **Standardization:** Features scaled using `StandardScaler` to ensure uniform gradient descent.
* **Label Encoding:** Categorical fruit names converted to numerical tensors.
* **Data Split:** 80% Training | 20% Testing.

### 🧠 Model Structure
The network is built using **PyTorch** with the following layers:
* **Input Layer:** 34 nodes (matching dataset features).
* **Hidden Layer 1:** 64 Neurons + ReLU Activation.
* **Hidden Layer 2:** 64 Neurons + ReLU Activation.
* **Output Layer:** 7 Neurons (representing fruit classes).

---

## 🚀 Performance
The model achieves impressive metrics on the test set:

| Metric | Value |
| :--- | :--- |
| **Accuracy** | **~94.44%** |
| **Loss Function** | Cross-Entropy Loss |
| **Optimizer** | Adam |
| **Epochs** | 100 |

---

## 📂 Project Structure
```bash
.
├── DateFruit_Dataset.csv     # Raw dataset
├── ANN_classification.ipynb  # Main training & evaluation logic
└── README.md                 # Project documentation
