Loan Approval Prediction
Project Overview

This project predicts whether a loan application will be approved or rejected based on applicant information using Machine Learning.
It demonstrates binary classification, handling imbalanced data, and comparing Logistic Regression and Decision Tree models.

Dataset

Source: Loan Approval Prediction Dataset (Kaggle)

Key columns:

loan_id – Unique identifier

education, self_employed – Categorical features

income_annum, loan_amount, loan_term, cibil_score – Numeric features

residential_assets_value, commercial_assets_value, luxury_assets_value, bank_asset_value – Asset values

loan_status – Target column (approved or rejected)

Data Preprocessing

Checked for missing values (none found)

Cleaned column names

Encoded categorical features using one-hot encoding

Encoded target column: approved = 1, rejected = 0

Split dataset into train/test sets (80/20) with stratification

Addressed class imbalance using SMOTE (Synthetic Minority Oversampling Technique)

Models

Logistic Regression – baseline model

Decision Tree Classifier – best-performing model

Evaluation Metrics

Precision, Recall, F1-score for each class

Confusion Matrix

Decision Tree achieved ~98% accuracy with balanced performance for both classes

Visualizations

Feature importance (Decision Tree)

Class distribution before & after SMOTE

Confusion matrix heatmaps
