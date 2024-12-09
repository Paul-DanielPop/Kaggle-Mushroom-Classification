# Mushroom Classification Project

This repository contains a comprehensive analysis of the **Mushroom Classification Problem**, where the objective is to predict whether a mushroom is **edible** or **poisonous** based on its physical characteristics. The project leverages various machine learning models and techniques to achieve high accuracy.

---

## 🔍 Problem Description

The dataset consists of various categorical features describing mushroom characteristics such as:
- Cap shape, surface, and color
- Bruising
- Odor
- Gill attachment, spacing, size, and color
- Stalk dimensions, surface, and color

The target variable is **class**, indicating whether the mushroom is:
- **Edible** (`e`)
- **Poisonous** (`p`)

---

## 🚀 Machine Learning Pipeline

### Preprocessing Steps
1. **Categorical Encoding**:
   - **Ordinal Encoding** for ordinal features.
   - **Frequency Encoding** for non-ordinal features to reduce dimensionality and improve performance.
2. **Feature Selection**:
   - Used **Mutual Information** with `SelectKBest` to identify the most relevant features.

### Models and Hyperparameter Tuning
The project implements multiple models using `GridSearchCV` for hyperparameter tuning:
- **Random Forest**
- **Logistic Regression**
- **Support Vector Machines (SVM)**
- **Gradient Boosting**
- **K-Nearest Neighbors (KNN)**

Each model is evaluated with metrics such as:
- **Confusion Matrix**
- **ROC/AUC Curve**
- **Precision-Recall Curve**

---

## 📊 Results and Insights

1. **Feature Importance**: Feature selection using mutual information highlighted key attributes contributing to the classification task.
2. **Model Performance**: The tuned models achieved high accuracy on the test set, with **Random Forest** and **Gradient Boosting** performing particularly well.
3. **Visualization**:
   - Confusion Matrix to understand prediction distributions.
   - ROC and Precision-Recall curves to evaluate model performance under different thresholds.

---

## 💡 Conclusions

1. Proper hyperparameter tuning and sufficient training data are crucial for achieving high classification performance.
2. Preprocessing steps like feature encoding and selection significantly impact the model's predictive accuracy.

---

## 📈 Future Improvements

- Experimenting with additional models, such as **Neural Networks**.
- Incorporating semi-supervised learning to handle potential missing labels in datasets.
- Testing model robustness with unseen and noisy data.

---

## 🛠️ Setup and Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/Paul-DanielPop/mushroom-classification.git
   cd mushroom-classification
2. Execute code (Python Installation and Packages required)
