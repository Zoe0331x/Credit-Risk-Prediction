# Credit-Risk-Prediction
Predicting loan default risk using Logistic Regression and LightGBM

💳 Loan Default Prediction for Female Borrowers

Heyy 🤸, I’m Zoe, and welcome to my project page 💕

This is a simplified version of my master’s thesis Loan Default Prediction for Female Borrowers: A Comparative Study on European P2P Lending Data.
It uses Python and machine learning to predict whether a female borrower is likely to default on a loan.
The notebook walks through data cleaning, feature creation, exploration, and two models: Logistic Regression and LightGBM.


🔎 Project Overview

In peer-to-peer lending, it’s important to know who might default before approving a loan.
This project focuses on female borrowers from the Bondora platform and builds a model to assess default risk.
The goal is to see how model complexity affects prediction performance.

The original thesis compared three models (Logistic Regression, XGBoost, and LightGBM) and included SHAP analysis.
Here, the focus is only on Logistic Regression and LightGBM to keep the workflow clear and easy to reproduce.


💡 Why Focus on Female Borrowers

Most credit risk models are trained on mixed or male-dominated datasets, assuming one-size-fits-all risk patterns.
However, research shows that female borrowers often have different financial behaviors. For example, more stable repayment patterns but smaller loan sizes.

This project focuses only on female borrower data to examine: if a model trained for women captures risk signals differently.

The goal is to highlight the importance of gender-sensitive credit modeling, especially for improving fairness and inclusiveness in financial decision-making.


🐈 Workflow

Step	Description

Data Cleaning	Keep only female borrowers and remove incomplete records

Feature Engineering	Create features like Payment-to-Income, Debt-to-Income, and Childbearing Age

EDA	Explore patterns such as default rate by education or loan duration

Modeling	Train Logistic Regression and LightGBM with 5-fold cross-validation

Evaluation	Compare metrics such as AUC, Precision, and Recall



📋 Dataset

The dataset comes from Bondora, a European P2P lending platform.
Each record represents one borrower and one loan application.

Main variables include:

Age

IncomeTotal

ExistingLiabilities

LoanDuration

Education

OccupationArea

HomeOwnershipType

LoanDefaulted (target variable)


🧠 Models
Model	Type	Description

Logistic Regression	Linear	Interpretable baseline

LightGBM	Tree-based	Captures non-linear patterns and interactions

LightGBM achieved higher AUC and recall, showing stronger performance in identifying defaults.


🌸 Future Work

Add XGBoost for a full comparison

Include parameter tuning (GridSearch or Optuna)

Apply SHAP to explain model predictions

