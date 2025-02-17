# Customer-Churn-Prediction---R-Data-Analytics
Customer Churn Prediction for a Telecommunications company using R Data Analytics
This repository contains an end-to-end implementation of customer churn prediction using logistic regression in R. The project analyzes key customer attributes to predict churn probability, evaluates model performance using ROC-AUC, and extracts business insights to improve retention strategies.

**Project Overview:**

The project follows these key steps:

1️⃣ **Data Loading & Exploration**
* Load customer data from Cellphone.xlsx
* Summarize dataset statistics
* Check for missing values

2️⃣ **Data Insights & Exploratory Analysis**
* Churn Rate Analysis: Count of churned vs. non-churned customers
* Monthly Charges & Churn: Boxplot analysis to check if higher monthly charges correlate with higher churn
* Tenure & Churn: Boxplot analysis to determine if customer loyalty impacts churn

3️⃣ **Train-Test Split**
* Convert data into a data frame
* Split data into 70% training and 30% testing using caret package

4️⃣ **Logistic Regression Model**
* Fit a logistic regression model with key predictor variables:
* AccountWeeks, ContractRenewal, DataPlan, DataUsage, CustServCalls, DayMins, DayCalls, MonthlyCharge
* Extract the logistic regression equation

5️⃣ **Model Performance Evaluation**
* Predict probabilities on test data
* ROC Curve Analysis: Evaluate model performance with AUC Score (0.817)
* Visualization: Plot ROC Curve using ggplot2


**Key Findings**
* Higher Monthly Charges increase the likelihood of churn.
* Contract Renewal is a strong predictor—customers with active renewals are less likely to churn.
* Tenure (AccountWeeks) alone is not a strong predictor of churn.
* AUC Score = 0.817 suggests a good predictive ability of the model.
