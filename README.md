# Credit Risk Prediction System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-0.95.0-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-orange)

An end-to-end machine learning application that evaluates a borrower's likelihood of loan repayment. This project features a **FastAPI** backend and a responsive frontend to provide real-time risk assessments.

## 🚀 Overview
Financial institutions use credit scoring to determine if a loan should be granted. This tool uses a **Random Forest Classifier** to analyze variables like income, loan intent, and credit history to predict risk categories.

## 🛠️ Tech Stack
- **Backend:** FastAPI, Uvicorn (ASGI server)
- **Machine Learning:** Scikit-learn, Pandas, Joblib
- **Frontend:** HTML5, CSS3, JavaScript (Fetch API)
<img width="1128" height="783" alt="Screenshot 2026-02-10 122312" src="https://github.com/user-attachments/assets/304057ee-9dae-4323-a9e8-d3cbe2c5c3f7" />



# Customer Churn Analysis (Exploratory Data Analysis Focus)

## Project Overview

This project investigates **customer churn behavior** in a telecom dataset.
The primary goal of this repository is not deployment or production modeling, but **understanding the data, identifying churn patterns, and deriving business insights**.

The machine learning model training was explored but intentionally paused. The focus here is on **analysis, feature relationships, and interpretation** rather than building a final production predictor.

---

## Objectives

* Understand which customers are most likely to churn
* Discover behavioral and billing patterns linked to churn
* Identify high‑risk customer profiles
* Provide business recommendations based on data

---

## Dataset Description

The dataset contains customer subscription information including:

* Customer tenure
* Monthly and total charges
* Contract type
* Payment method
* Internet service type
* Additional services (streaming, security, backup, etc.)
* Churn label (Yes / No)

---

## Exploratory Data Analysis (EDA)

### 1. Class Imbalance

* Churned customers are significantly fewer than retained customers
* This affects model behavior and evaluation metrics

**Implication:** Accuracy alone is misleading — recall for churn matters more.

---

### 2. Tenure

Observation:

* New customers churn far more often
* Long‑term customers rarely churn

**Insight:** The first months are the critical retention window.
<img width="1378" height="439" alt="Screenshot 2026-02-17 143317" src="https://github.com/user-attachments/assets/1dd00e63-ca57-47d6-8e45-51831d78791e" />

---

### 3. Contract Type

Observation:

* Month‑to‑month customers churn the most
* Two‑year contracts churn the least
<img width="895" height="517" alt="Screenshot 2026-02-17 143040" src="https://github.com/user-attachments/assets/8854fc6d-7439-4e11-955e-059e1e2f020f" />

**Business Meaning:** Commitment reduces churn risk dramatically

---

### 4. Charges & Spending Behavior

Key patterns discovered:

* High monthly charges → higher churn probability
* Low tenure + high bill = highest risk group
* Average monthly spend strongly correlates with churn
<img width="842" height="754" alt="Screenshot 2026-02-17 142541" src="https://github.com/user-attachments/assets/278ec5d0-cd29-44f1-afc9-9ba25db6a868" />

---

### 5. Payment Method

Electronic check users churn more than other payment methods.

**Possible interpretation:**
Customers using less automated payment methods may be less committed or less satisfied.

---

### 6. Internet Service Type

Fiber optic customers show higher churn despite paying more.

<img width="1277" height="693" alt="image" src="https://github.com/user-attachments/assets/86a1fe68-c5bf-4185-9077-3ea5a0a7d443" />

**Possible reason:**
Higher expectations → dissatisfaction leads to churn

---

<img width="856" height="661" alt="Screenshot 2026-02-17 143235" src="https://github.com/user-attachments/assets/b306c8a1-38c2-40de-af93-50841108d9a9" />




**Key takeaway:** Pricing + commitment length dominate churn behavior more than extra services.

---

## High‑Risk Customer Profile

A typical churn‑risk customer:

* New customer
* Month‑to‑month contract
* High monthly bill
* Fiber internet user
* Pays with electronic check

---

## Business Recommendations

1. Focus retention efforts on first 3 months
2. Incentivize long‑term contracts early
3. Offer onboarding discounts for high monthly charges
4. Improve service experience for fiber customers
5. Encourage automatic payment methods

---

## Machine Learning (Work in Progress)

Initial models were tested for exploration only:

* Logistic Regression
* Random Forest
* Threshold tuning
* Probability calibration

The model is intentionally not finalized. This repository prioritizes **understanding over prediction accuracy**.

Future work may include:

* Production‑ready pipeline
* API deployment
* Real‑time predictions

---

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib / Seaborn
* Scikit‑learn
* Google Colab / Jupyter Notebook

---

## Author Note

This project serves as a learning exploration in data analysis and interpretation.
The goal is to practice thinking like a data analyst: extracting meaning from data rather than just training models.
