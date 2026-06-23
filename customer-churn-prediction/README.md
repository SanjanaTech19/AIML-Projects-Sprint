# 📊 Customer Churn Prediction

This repository contains an end-to-end machine learning project designed to predict customer churn and identify at-risk users before they leave the service.

## 📝 About the Project

Customer churn occurs when customers stop doing business with a company or stop using its services. Retaining existing customers is significantly cheaper than acquiring new ones, making churn prediction a high-priority business requirement.

This project addresses the problem by analyzing historical customer behaviors, account attributes, and demographics. By training a classification model, the project helps businesses flag high-risk customers and deploy targeted incentive or marketing campaigns to maximize customer retention.

### Key Objectives:
*   Perform Exploratory Data Analysis (EDA) to find major churn drivers.
*   Handle class imbalance using advanced oversampling techniques.
*   Train, evaluate, and compare multiple classification algorithms.
*   Deploy a lightweight web interface for real-time model inference.


## 🛠️ Tools and Technologies Used

The project is built entirely in **Python** using the following stack:

*   Data Manipulation: NumPy & Pandas
*   Data Visualization: Matplotlib & Seaborn
*   Machine Learning: Scikit-Learn

## 📅 About the Dataset

The model utilizes the popular Telco Customer Churn dataset (commonly sourced from Kaggle). It contains structured profiles of 7,043 unique customers with 21 distinct features.

### Target Variable:
*   Churn: Indicates whether the customer left within the last month (Yes or No).

### Feature Breakdowns:
1.  Demographic Information:
    *   gender: Male or Female.
    *   SeniorCitizen: Whether the customer is a senior citizen (1, 0).
    *   Partner / `Dependents`: Whether the customer has a partner or dependents (Yes, No).
2.  Customer Account Data:
    *   tenure: Number of months the customer has stayed with the company.
    *   Contract: The contract term type (Month-to-month, One year, Two year).
    *   PaperlessBilling: Whether paperless billing is enabled (Yes, No).
    *   PaymentMethod: Electronic check, Mailed check, Bank transfer, Credit card.
    *   MonthlyCharges: The amount charged to the customer monthly.
    *   TotalCharges: The total amount charged to the customer.
3.  Services Subscribed:
    *   Phone service, multiple lines, internet service provider, online security, online backup, device protection, tech support, and streaming TV/movies.
