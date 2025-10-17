Loan Approval Prediction
Overview

This project predicts whether a loan application will be approved based on applicant financial and personal information. It demonstrates real-world machine learning techniques including binary classification, handling imbalanced datasets, and model evaluation using Logistic Regression and Decision Tree models.

Dataset

The dataset contains historical loan applications with the following key features:

loan_id – Unique application identifier

education, self_employed – Categorical applicant information

income_annum, loan_amount, loan_term, cibil_score – Financial metrics

residential_assets_value, commercial_assets_value, luxury_assets_value, bank_asset_value – Asset values

loan_status – Target variable (approved or rejected)

Source: Kaggle Loan Approval Prediction Dataset

Data Preprocessing

Cleaned column names and standardized values

One-hot encoded categorical features

Encoded the target column: approved = 1, rejected = 0

Split data into training (80%) and testing (20%) sets with stratification

Addressed class imbalance using SMOTE (Synthetic Minority Oversampling Technique)

Models

Logistic Regression – baseline model for comparison

Decision Tree Classifier – best-performing model

Evaluation Metrics: Precision, Recall, F1-score, Confusion Matrix

Decision Tree achieved ~98% accuracy, with balanced performance for both approved and rejected applications

Visualizations

Feature importance from Decision Tree

Class distribution before and after SMOTE

Confusion matrices for each model

How to Run

Clone the repository:

git clone https://github.com/<your-username>/loan-approval-prediction.git


Navigate to the project folder:

cd loan-approval-prediction


Install dependencies:

pip install -r requirements.txt


Open the notebook:

jupyter notebook notebooks/Loan_Approval_Prediction.ipynb

Requirements

Python 3.x

pandas

scikit-learn

imbalanced-learn

matplotlib

Future Work

Hyperparameter tuning for Decision Tree

Explore ensemble methods like Random Forest and XGBoost

Deploy as a web application for real-time loan predictions
