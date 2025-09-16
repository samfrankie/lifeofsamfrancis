# Customer Churn Prediction

## Project Overview

This project aims to build a predictive model to identify customers who are likely to churn (i.e., cancel their service) for a telecommunications company. By proactively identifying at-risk customers, the business can implement targeted retention strategies, such as special offers or personalized support, to improve customer lifetime value and reduce churn rates.

---

## The Business Problem

Customer churn is a significant challenge for subscription-based businesses. It's often more expensive to acquire a new customer than to retain an existing one. Predicting which customers are likely to leave allows a company to intervene before it's too late.

The model will help answer key business questions like:
- Which customers are most likely to churn in the near future?
- What factors are the strongest predictors of churn?
- What are the characteristics of high-risk customer segments?

---

## Methodology

The project follows a standard machine learning pipeline:

1.  **Data Collection**: Utilized a publicly available dataset containing customer information and a churn status.
2.  **Data Cleaning & Preprocessing**: Handled missing values, converted categorical features to numerical ones using one-hot encoding, and scaled numerical data.
3.  **Exploratory Data Analysis (EDA)**: Analyzed customer demographics, service usage, and contract details to uncover relationships with churn. 
4.  **Feature Engineering**: Created new features, such as `TotalCharges` and `MonthlyCharges`, to provide more predictive power to the model.
5.  **Model Building**:
    - Split the data into training and testing sets.
    - Trained a **Random Forest Classifier**, which is well-suited for this type of classification problem.
    - Evaluated the model using a **confusion matrix**, **classification report**, and **ROC curve**.
6.  **Results & Interpretation**: Analyzed the model's performance and extracted feature importance scores to understand which variables most influence a customer's decision to churn.

---

## Key Findings

- **Contract Type** and **Monthly Charges** were found to be among the strongest predictors of churn. Customers on month-to-month contracts and those with higher monthly fees were significantly more likely to churn.
- The **Random Forest model** achieved a high prediction accuracy, outperforming a baseline model.
- The insights gained can be used to inform business strategies, such as offering long-term contracts to at-risk customers or adjusting pricing models.

---

## Technologies Used

- **Python**: Core programming language.
- **Pandas** & **NumPy**: For data manipulation and numerical operations.
- **Scikit-learn**: For machine learning modeling and evaluation.
- **Matplotlib** & **Seaborn**: For data visualization.
- **Jupyter Notebook**: For reproducible analysis.
