# Adey Innovations Inc. Fraud Detection Project

## Overview

This project aims to improve fraud detection for e-commerce and banking transactions using advanced data analysis, feature engineering, machine learning, and model explainability. The solution is designed to balance security and user experience, minimize financial loss, and build customer trust.

## Project Structure

- `data/` – Raw datasets (`Fraud_Data.csv`, `IpAddress_to_Country.csv`, `creditcard.csv`)
- `notebooks/` – Jupyter notebooks for data analysis, modeling, and explainability
- `src/` – Python scripts for preprocessing and modeling (optional for automation)
- `reports/` – Professional interim and final reports for business and technical stakeholders

## Tasks and Workflow

### Task 1: Data Analysis and Preprocessing

- Data cleaning, handling missing values, and removing duplicates
- Exploratory Data Analysis (EDA) with visualizations and documentation
- Feature engineering (transaction frequency, time-based features, geolocation)
- Data transformation (encoding, normalization, SMOTE for class imbalance)

### Task 2: Model Building and Training

- Train-test split and SMOTE for balanced training data
- Model selection: Logistic Regression (baseline) and Random Forest (ensemble)
- Model evaluation using F1-score, AUC-PR, and confusion matrix
- Model comparison and business justification

### Task 3: Model Explainability

- SHAP analysis for global and local interpretability
- Summary, beeswarm, force, dependence, and waterfall plots
- Translation of technical insights into business value

## Key Results

- **Random Forest** outperformed Logistic Regression in both F1-score and AUC-PR on both datasets.
- **SHAP analysis** revealed key fraud drivers, supporting business understanding and operational integration.

## Reports

- `reports/interim_report.md` – Progress, methodology, EDA, and next steps
- `reports/final_report.md` – Full project documentation, results, SHAP insights, and recommendations

## How to Use

1. Place datasets in the `data/` folder.
2. Run notebooks in `notebooks/` for each task.
3. Review professional reports in `reports/` for business and technical summaries.

## Business Value

This project enables Adey Innovations Inc. to:

- Detect fraud more accurately and efficiently
- Reduce financial losses and false positives
- Build trust with customers and partners
- Provide actionable insights for fraud investigation and business strategy

---
