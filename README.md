# 🏦 Bank Loan Default Prediction — Logistic Regression

## 📌 Overview

This project builds a simple **AI/ML model using Logistic Regression** to predict whether a loan applicant is likely to **default (fail to repay)** or **repay** their loan.

The project uses a realistic **synthetic dataset** because real bank loan data is private and regulated. Logistic Regression was selected because it is easy to explain, transparent, and provides a coefficient (weight) for each feature.

## 🎯 Objective

The main objective is to identify applicants who have a higher risk of loan default and help support **credit-risk assessment**.

## 📊 Dataset

The notebook creates a synthetic dataset containing **3,000 loan applicants**. Each applicant includes financial, credit, employment, and loan information.

### Features

* `annual_income` — Applicant's annual income in thousands
* `credit_score` — Credit score between 300 and 850
* `loan_amount` — Requested loan amount in thousands
* `debt_to_income` — Existing monthly debt payments as a percentage of monthly income
* `employment_years` — Years at the current job
* `late_payments_2yr` — Number of late payments in the last 2 years
* `loan_purpose` — Home, Auto, or Personal
* `default` — Target variable: `1 = Defaulted`, `0 = Repaid`

## 🤖 Machine Learning Model

**Algorithm:** Logistic Regression
**Type:** Supervised Binary Classification
**Target:** Loan Default

The model learns patterns from the applicant data and predicts whether an applicant is likely to default.

## 🔄 Workflow

1. Import required Python libraries.
2. Generate the synthetic loan applicant dataset.
3. Explore the dataset and default rate.
4. Convert `loan_purpose` using one-hot encoding.
5. Split the data into **80% training** and **20% testing** sets.
6. Standardize the numerical features using `StandardScaler`.
7. Train the Logistic Regression model.
8. Evaluate the predictions using accuracy and a classification report.
9. Generate a confusion matrix.
10. Analyze model coefficients to understand which features influence default risk.
11. Test the model on individual applicants.

## 📈 Model Evaluation

The model uses:

* Accuracy
* Classification Report
* Confusion Matrix

The notebook also displays the model's feature weights to understand which factors push an applicant toward **default** or **repayment**.

## 🔍 Key Findings

The model indicates that:

* **Lower credit scores** increase default risk.
* **More late payments** increase default risk.
* **Higher income** reduces default risk.
* **Longer employment tenure** reduces default risk.
* **Lower debt-to-income ratios** reduce default risk.

## 💼 Business Use

A bank could use a similar model to identify high-risk applicants and route them for additional **manual underwriting review**.

The model could also support decisions such as offering a smaller loan amount or adjusting interest rates according to risk.

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook
* Logistic Regression
* StandardScaler

## 📁 Repository Structure

```text
bank-loan-default-prediction/
│
├── bank_loan_default_logistic_regression-2.ipynb
└── README.md
```

## ⚠️ Disclaimer

This project is intended for **educational purposes** an
