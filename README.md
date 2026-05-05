#  Fraud Detection System using Machine Learning

##  Overview

This project develops a **fraud detection (transaction risk scoring) system** using supervised machine learning techniques. The goal is to accurately identify fraudulent financial transactions within an imbalanced dataset while maintaining a balance between detecting fraud and minimizing false positives.

The project follows a complete machine learning pipeline including:

* Data preprocessing
* Feature engineering
* Handling class imbalance
* Model training and evaluation
* Model validation and interpretability

---

##  Objectives

* Detect fraudulent transactions using classification models
* Handle imbalanced financial data effectively
* Evaluate model performance using appropriate metrics (F1-score, ROC-AUC)
* Provide interpretable insights into key fraud-driving features

---

##  Dataset

* Dataset: `bs140513_032310.csv`
* Contains anonymised bank transaction data
* Target variable: `fraud` (binary classification)

---

##  Tech Stack

* **Languages**: Python
* **Libraries**:

  * pandas, numpy
  * scikit-learn
  * imbalanced-learn (SMOTE)
  * matplotlib, seaborn

---

##  Project Pipeline

### 1. Data Preprocessing

* Train-test split (stratified)
* Label encoding for categorical variables (avoiding data leakage)
* Feature scaling using StandardScaler

### 2. Handling Imbalanced Data

* Applied **SMOTE (Synthetic Minority Oversampling Technique)** on training data only

### 3. Model Development

* Random Forest Classifier (primary model)
* Logistic Regression (baseline comparison)

### 4. Model Evaluation

* Accuracy
* Precision & Recall
* F1-score
* ROC-AUC score
* Confusion Matrix
* ROC Curve

### 5. Model Validation

* 5-fold Cross-validation (F1-score)

### 6. Model Interpretability

* Feature importance analysis to identify key fraud indicators

---

##  Key Results

| Metric   | Score (Random Forest) |
| -------- | --------------------- |
| Accuracy | 0.98                  |
| F1 Score | 0.63                  |
| ROC-AUC  | ~0.90+                |

>  Note: Accuracy is high due to class imbalance; F1-score and ROC-AUC are more meaningful metrics.

---

##  Key Insights

* Handling class imbalance significantly improves fraud detection performance
* Threshold tuning helps balance false positives vs false negatives
* Feature importance reveals key drivers of fraudulent behaviour
* Random Forest outperforms Logistic Regression for this dataset

---

##  Future Improvements

* Hyperparameter tuning (GridSearch / RandomSearch)
* Use of advanced models (XGBoost, LightGBM)
* Pipeline integration for production deployment
* SHAP values for deeper explainability
* Real-time fraud detection system

---

##  Business Relevance

This project simulates real-world financial risk modelling systems used in:

* Fraud detection
* Credit risk scoring
* Transaction monitoring

Such systems are critical in improving financial security and enabling data-driven decision-making in fintech environments.

---

##  Contact

If you'd like to discuss this project or collaborate, feel free to connect!

---
