# Neural Network and Random Forest for Imbalanced Dataset Classification

This repository contains the implementation of supervised machine learning models, specifically **Neural Networks** and **Random Forests**, to predict whether a client will subscribe to a term deposit. The project handles imbalanced data using **oversampling techniques (SMOTE)** and **undersampling the majority class**. It provides end-to-end data preprocessing, feature engineering, model training, evaluation, and optimization.

---

## **Objective**

To make accurate predictions about whether a client will subscribe to term deposits based on the dataset from the UCI Bank Marketing Repository. This information helps banks make informed decisions regarding term deposit services, customer targeting, and overall financial strategies.

---

## **Dataset Overview**

- **Source:** [UCI Bank Marketing Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
- **Rows:** 45,211
- **Features:**
  - **Categorical:** job, marital, education, default, housing, loan, contact, month, poutcome, y
  - **Numerical:** age, day, balance, duration, campaign, pdays, previous

The target variable (`y`) indicates whether the client subscribed to the term deposit:
- `yes`: 1
- `no`: 0

---

## **Key Features**

- **Data Preprocessing:**
  - Handling missing values and outliers.
  - One-hot encoding for categorical features.
  - Dropping irrelevant features (`default`, `pdays`, etc.).
  - Correlation analysis to avoid multicollinearity.
  - Feature scaling for numerical data.

- **Class Balancing Techniques:**
  - **SMOTE:** Oversamples the minority class by generating synthetic samples.
  - **RandomUnderSampler:** Undersamples the majority class to match the size of the minority class.

- **Models Implemented:**
  - **Neural Network:**
    - Two hidden layers (128 and 64 neurons) with ReLU activation.
    - Output layer with sigmoid activation for binary classification.
    - Achieved 89% accuracy.
  - **Random Forest:**
    - Hyperparameter tuning for `n_estimators`, `max_depth`, and `min_samples_split`.
    - Achieved 90% accuracy with feature importance analysis.

- **Evaluation Metrics:**
  - Confusion Matrix
  - Classification Report (Precision, Recall, F1-score)
  - ROC-AUC Score
  - Threshold tuning for optimized classification.

---

- **Contact Details:**
- Name-Akshan Kumarasan
- Email-Akshan.20222376@iit.ac.lk
