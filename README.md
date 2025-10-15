# 🎯 Predicting Loan Default Risk using Logistic Regression and LightGBM

📌 **Thesis Project: Loan Default Prediction for Female Borrowers**  
*Master’s in Data Science – Tilburg University*

---

## 🧠 Overview

This project presents a simplified version of my master’s thesis:  
**“Loan Default Prediction for Female Borrowers: A Comparative Study on European P2P Lending Data.”**

The notebook demonstrates how to use Python and machine learning to predict whether a female borrower is likely to default on a loan. It walks through:

- Data cleaning and preprocessing  
- Feature engineering  
- Exploratory data analysis (EDA)  
- Model training using Logistic Regression and LightGBM  
- Evaluation using AUC, precision, recall

The original thesis also included XGBoost and SHAP analysis. For simplicity, this repo focuses on two models: **Logistic Regression** and **LightGBM**.

---

## 💡 Motivation: Why Focus on Female Borrowers?

Traditional credit risk models often rely on mixed or male-dominated data. However, research indicates female borrowers may exhibit different financial behaviors — e.g., smaller loan sizes but more stable repayment patterns.

By focusing solely on female borrowers, this project explores whether tailored credit models can improve **fairness and prediction quality** in financial decision-making.

---

## 🔄 Workflow Summary

| Step               | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| Data Cleaning       | Filter female borrowers, remove incomplete records                         |
| Feature Engineering | Create variables: Payment-to-Income, Debt-to-Income, Childbearing Age      |
| EDA                 | Visualize default rates by education, duration, etc.                        |
| Modeling            | Train Logistic Regression and LightGBM with 5-fold cross-validation         |
| Evaluation          | Compare AUC, precision, recall                                              |

---

## 📊 Dataset

Sourced from **Bondora**, a European peer-to-peer lending platform.

Each row = one borrower’s loan application.  
Main variables:

- `Age`  
- `IncomeTotal`  
- `ExistingLiabilities`  
- `LoanDuration`  
- `Education`  
- `OccupationArea`  
- `HomeOwnershipType`  
- `LoanDefaulted` *(Target variable)*

---

## 🔍 Models Used

| Model               | Type        | Notes                                           |
|--------------------|-------------|--------------------------------------------------|
| Logistic Regression | Linear      | Interpretable baseline                          |
| LightGBM            | Tree-based  | Captures nonlinear patterns and interactions    |

✅ **LightGBM** showed higher AUC and better recall, indicating better performance in identifying defaults.

---

## 🌱 Future Work

- Add **XGBoost** for complete comparison  
- Apply **hyperparameter tuning** (e.g., GridSearch, Optuna)  
- Integrate **SHAP** for model explainability  
- Explore **gender-balanced** model comparisons

---

## 🔧 Tech Stack

- Python (Pandas, Scikit-learn, LightGBM)  
- Jupyter Notebook  
- Matplotlib / Seaborn for EDA  

---

## 👩 Author

**Zoe Xia**  
> MSc Data Science and Society | Power BI & Databricks Certified  
> 💼 [linkedin.com/in/zoexia](https://www.linkedin.com/in/zoe-xia-4b6307132/)
> 📂 [More projects on GitHub](https://github.com/Zoe0331x)

