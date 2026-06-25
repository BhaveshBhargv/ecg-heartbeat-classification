# 🫀 ECG Heartbeat Multiclass Classification

A deep learning project that classifies ECG heartbeat signals into multiple cardiac categories using a **1D Convolutional Neural Network (CNN)**, achieving **97% accuracy**.

Built as part of the MSc Advanced Data Science programme at the University of Exeter.

---

## 📋 Project Overview

Electrocardiogram (ECG) signals carry critical information about heart health. This project frames heartbeat classification as a **multiclass supervised learning problem**, training a 1D CNN to distinguish between different cardiac rhythm categories from raw time-series signal data.

---

## 🎯 Results

| Metric | Score |
|--------|-------|
| Accuracy | **97%** |
| Validation Strategy | K-Fold Cross-Validation |
| Model | 1D Convolutional Neural Network |

---

## 🗂️ Dataset

The dataset was provided as part of university coursework and contains labelled ECG signal recordings across multiple heartbeat categories (e.g. normal, and various arrhythmia types).

Each sample is a fixed-length time series representing a single heartbeat, with a corresponding class label for supervised classification.

---

## 🔧 Methodology

### 1. Data Preprocessing
- **Shuffling** — randomised sample order to remove ordering bias before splitting
- **Class balancing** — handled class distribution to prevent the model from being biased toward majority categories
- **Normalisation** — scaled signal values for stable neural network training

### 2. Model Architecture
- **1D CNN** built with TensorFlow / Keras
- Convolutional layers to extract local temporal features from the ECG signal
- Pooling layers for dimensionality reduction
- Dense output layer with softmax activation for multiclass classification

### 3. Training & Evaluation
- **K-Fold Cross-Validation** to ensure robust and reliable performance estimates
- **Hyperparameter tuning** to optimise architecture (number of filters, kernel size, learning rate, dropout rate)
- Evaluated using accuracy and cross-validation scores across all folds

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| TensorFlow / Keras | 1D CNN model design and training |
| scikit-learn | K-Fold cross-validation, preprocessing, metrics |
| NumPy / pandas | Data manipulation and analysis |
| Matplotlib / Seaborn | Visualisation of results and signal plots |

---

## 📁 Project Structure

```
ecg-heartbeat-classification/
│
├── ecg_classification.ipynb   # Main Colab notebook
├── mitbih_test.csv            # Test Dataset
├── mitbih_train.csv           # Train Dataset
└── README.md                  # Project documentation
```

---

## 🚀 Getting Started

### Run in Google Colab
Click the badge below to open the notebook directly in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vGM_BGqZKK1QQaKAiI9WiYEeu7yS5xVq#scrollTo=DgXc7E_iRo_x)

### Run Locally
```bash
# Clone the repository
git clone https://github.com/BhaveshBhargv/ecg-heartbeat-classification.git
cd ecg-heartbeat-classification

# Open the notebook
jupyter notebook ecg_classification.ipynb
```

---

## 📦 Requirements

```
tensorflow>=2.x
scikit-learn
numpy
pandas
matplotlib
seaborn
jupyter
```

---

## 🎓 Academic Context

- **Programme:** MSc Advanced Data Science, University of Exeter
- **Type:** Coursework Project
- **Key Concepts:** Deep Learning, 1D CNN, Time-Series Classification, K-Fold Cross-Validation, Hyperparameter Tuning

---

## 👤 Author

**Bhavesh Bhargava**
[LinkedIn](https://www.linkedin.com/in/bhavesh-bhargava-80ab2a10b/) · [GitHub](https://github.com/BhaveshBhargv/)
