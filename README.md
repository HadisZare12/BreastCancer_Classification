# 🧠 Breast Cancer Classification with PyTorch

This project builds and evaluates a **feedforward neural network** to classify breast tumors as **malignant** or **benign** using the **UCI Breast Cancer Wisconsin dataset**.  
It demonstrates **deep learning for healthcare diagnostics** with a focus on accuracy, interpretability, and reproducibility.

---

## 📌 Overview

Early and accurate diagnosis of breast cancer is critical for effective treatment.  
Using patient clinical data, this project trains a **neural network in PyTorch** to assist in predicting tumor malignancy.

---

## 📊 Dataset

- **Source:** [UCI Breast Cancer Wisconsin Dataset](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html)  
- **Samples:** 569  
- **Features:** 30 numeric features (e.g., radius mean, texture mean, smoothness, compactness)  
- **Target:** `0` = Malignant, `1` = Benign  

---

## 🛠️ Methodology

1. **Data Preprocessing**
   - Loaded dataset from `scikit-learn`
   - Standardized features with `StandardScaler`
   - Train/test split (80% / 20%)

2. **Model Architecture**
   - Input layer: 30 neurons (one per feature)
   - Hidden layer: 1 dense layer with ReLU activation
   - Output layer: 1 neuron with sigmoid activation (binary classification)

3. **Training**
   - Loss: Binary Cross-Entropy
   - Optimizer: Adam
   - Epochs: 100
   - Batch size: 32

4. **Evaluation**
   - Accuracy score
   - ROC curve and AUC
   - Confusion matrix

---

## 🚀 Results

- **Accuracy:** ~98% on test set  
- **ROC AUC:** ~0.995  
- High recall for malignant cases, reducing false negatives

---
## 💻 Installation & Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/HadisZare12/breast-cancer-classification.git
   cd breast-cancer-classification

