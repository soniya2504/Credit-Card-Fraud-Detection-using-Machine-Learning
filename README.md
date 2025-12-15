Project Overview

Credit card fraud is a major challenge for the banking and fintech industry. The goal of this project is to build a reliable and interpretable fraud detection system that can:

Accurately identify fraudulent transactions

Minimize financial losses

Reduce false positives to maintain good customer experience

Provide explainable predictions for business trust

This project follows a complete real-world ML workflow, from raw data to a saved production-ready model.

 Dataset Information

Source: Kaggle – Credit Card Fraud Detection Dataset

Observations: 284,807 transactions

Fraud Cases: 492 (≈ 0.17%)

Features:

V1 to V28 – PCA-transformed features

Time – Seconds elapsed between each transaction

Amount – Transaction amount

Class – Target variable

1 → Fraud

0 → Non-Fraud

 The dataset is extremely imbalanced, making it ideal for real-world fraud modeling.

 Tools & Technologies Used

Programming Language: Python

Libraries:

pandas, numpy – Data handling

matplotlib, seaborn – Visualization

scikit-learn – ML models & evaluation

imbalanced-learn (SMOTE) – Class imbalance handling

xgboost / GradientBoosting – Advanced ML model

shap – Model explainability

joblib – Model & pipeline saving

 Project Workflow

Environment Setup

Data Loading & Inspection

Problem Definition

Exploratory Data Analysis (EDA)

Data Preprocessing

Handling Class Imbalance using:

Class Weighting

SMOTE Oversampling

Model Training:

Logistic Regression

Random Forest

Gradient Boosting / XGBoost

Model Evaluation using:

Confusion Matrix

Precision, Recall, F1-score

ROC-AUC, PR-AUC

Model Comparison & Selection

Feature Importance & Explainability (SHAP & Coefficients)

Threshold Optimization

Final Model Saving & Deployment-ready Predictions

 Key Evaluation Metrics

Since fraud detection is a high-risk classification problem, the following metrics were prioritized:

 Recall (Most Important) – To minimize missed frauds

 F1-Score – Balance between precision & recall

 ROC-AUC – Overall separability

 PR-AUC – Performance on imbalanced data

 Accuracy alone was not used due to extreme class imbalance.

 Best Model Selection

The final model was selected based on:

Highest Recall

Strong F1-score

Best ROC-AUC & PR-AUC


 Model Explainability

Feature Importance from tree-based models

Logistic Regression coefficients

SHAP explainability was attempted:

PCA-transformed features and pipelines caused compatibility limitations

Model interpretation was successfully handled using traditional techniques.
...........................................................................
...........................................................................
