# INTERIM REPORT

## Introduction – Project Overview and Understanding

Adey Innovations Inc. is a leader in financial technology, providing secure solutions for e-commerce and banking. Fraud detection is a critical business need: undetected fraud leads to financial loss and erodes customer trust, while excessive false positives can harm user experience. This project aims to develop robust, interpretable machine learning models to accurately identify fraudulent transactions, leveraging transaction data, user/device behavior, and geolocation information.

## Methodology – Process, Progress, and Results

### Data Understanding and Preparation

- **Datasets Used:**

  - `Fraud_Data.csv`: E-commerce transaction data with user, device, and transaction details.
  - `IpAddress_to_Country.csv`: Maps IP address ranges to countries.
  - `creditcard.csv`: Bank transaction data with anonymized features.

- **Data Preprocessing:**
  - **Missing Values & Duplicates:** All missing values and duplicates were removed to ensure data quality.
  - **Data Types:** Timestamps and categorical variables were converted to appropriate formats.
  - **Feature Engineering:** Created features such as transaction frequency per user, time since signup, hour of day, and day of week.
  - **Geolocation:** Merged geolocation data by mapping IP addresses to countries, enabling country-level fraud analysis.

### Exploratory Data Analysis (EDA) Insights and Documentation

- **Class Imbalance:** Both datasets are highly imbalanced, with far fewer fraudulent transactions than legitimate ones. This was visualized and quantified.
- **Feature Distributions:** Fraudulent transactions often have distinct patterns in purchase value, transaction timing, and user behavior.
- **Geolocation:** Certain countries and IP ranges are more associated with fraud, as revealed by merging and analyzing geolocation data.
- **EDA Documentation:** Plots and statistical summaries were generated for all key features, and findings were documented to guide feature engineering and model selection.

### Data Preprocessing: Cleaning and Feature Engineering

- **Categorical Encoding:** Applied one-hot encoding to categorical features.
- **Normalization:** Used `StandardScaler` for normalization of numerical features.
- **Class Imbalance:** Addressed using SMOTE (Synthetic Minority Over-sampling Technique) to balance the training data.

### Model Building and Training

- **Models Compared:**
  - Logistic Regression (baseline, interpretable)
  - Random Forest (ensemble, powerful)
- **Evaluation Metrics:** F1-score, AUC-PR, and confusion matrix, focusing on performance for imbalanced data.
- **Results:** Random Forest consistently outperformed Logistic Regression in both F1-score and AUC-PR on both datasets.

## Challenges & Solutions

- **Severe Class Imbalance:** Addressed using SMOTE and by selecting appropriate evaluation metrics.
- **Feature Engineering:** Required careful handling of timestamps, categorical variables, and merging external geolocation data.
- **Interpretability vs. Performance:** Balanced by using both interpretable (Logistic Regression) and powerful (Random Forest) models.
- **Technical Communication:** All steps, code, and findings were documented in Jupyter notebooks with clear markdown explanations and visualizations.

## Future Plan

- **Model Explainability:** Apply SHAP to interpret the best-performing model and communicate key fraud drivers.
- **Business Translation:** Translate technical findings into actionable business insights for stakeholders.
- **Final Evaluation:** Refine models, document insights, and prepare a comprehensive final report with recommendations.

## Conclusion

Significant progress has been made in data cleaning, feature engineering, and model development. The project is on track, with strong initial results from Random Forest models. The next steps will focus on explainability and business value translation, ensuring the solution is both accurate and actionable for Adey Innovations Inc.

---
