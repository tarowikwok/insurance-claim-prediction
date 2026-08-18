# 🛡️ Insurance Claim Prediction & Risk Analysis

> A machine learning application for predicting insurance claim probability and analyzing customer risk levels through an interactive Streamlit dashboard.

![Python](https://img.shields.io/badge/Python-3.13-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Scikit Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E?logo=scikitlearn)
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?logo=streamlit)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📌 Overview

**Insurance Claim Prediction & Risk Analysis** is an end-to-end machine learning project designed to predict the likelihood of an insurance claim and transform the prediction into an actionable customer risk classification.

The system analyzes customer, policy, vehicle, claim history, and driving behavior data to estimate the probability of a future insurance claim.

The prediction is then converted into three risk categories:

| Claim Probability | Risk Level |
|---:|:---|
| < 30% | 🟢 LOW |
| 30% – 69% | 🟡 MEDIUM |
| ≥ 70% | 🔴 HIGH |

The project includes an interactive **Streamlit dashboard** that allows users to perform individual predictions, explore customer risk profiles, evaluate machine learning models, and inspect the underlying dataset.

---

# 🎯 Business Problem

Insurance companies need to evaluate customer risk efficiently while handling large amounts of policy and customer data.

Traditional risk assessment can be time-consuming and may rely heavily on manual evaluation.

This project demonstrates how machine learning can support insurance risk assessment by:

- Predicting the probability of an insurance claim
- Identifying potentially high-risk customers
- Segmenting customers based on predicted claim probability
- Analyzing factors associated with claim risk
- Providing a centralized interactive dashboard for decision support

> **Note:** This application is a machine learning decision-support prototype and is not intended to replace professional insurance underwriting or regulatory decisions.

---

# 💡 Solution

The system follows an end-to-end machine learning workflow:

```text
Insurance Dataset
       │
       ▼
Data Preparation
       │
       ▼
Feature Engineering
       │
       ▼
Train / Test Split
       │
       ▼
Model Training
       │
       ├───────────────┐
       ▼               ▼
Logistic Regression  Random Forest
       │               │
       └───────┬───────┘
               ▼
       Model Evaluation
               │
               ▼
         Best Model
               │
       ┌───────┴────────┐
       ▼                ▼
Claim Prediction    Risk Analysis
       │                │
       ▼                ▼
Probability       LOW / MEDIUM / HIGH
       │
       ▼
Streamlit Dashboard