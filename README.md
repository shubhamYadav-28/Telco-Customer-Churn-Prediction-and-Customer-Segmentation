# Telco-Customer-Churn-Prediction-and-Customer-Segmentation

## Project Overview

Customer churn is a critical challenge for telecom companies as losing customers directly impacts revenue and growth. This project focuses on predicting customer churn using Machine Learning and identifying customer segments through clustering techniques to support data-driven business decisions.

The project combines **Random Forest Classification** for churn prediction and **K-Means Clustering** for customer segmentation.

---

## Dataset

**Dataset:** Telco Customer Churn Dataset

The dataset contains customer information such as:

* Customer tenure
* Monthly charges
* Total charges
* Contract type
* Internet service type
* Payment method
* Technical support status
* Customer Lifetime Value (CLTV)
* Churn information

---

## Objectives

* Analyze customer behavior and churn patterns.
* Predict whether a customer is likely to churn.
* Identify the factors contributing to churn.
* Evaluate model performance using multiple metrics.
* Segment customers into meaningful business groups.
* Generate actionable insights for customer retention strategies.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* OpenPyXL

---

## Exploratory Data Analysis (EDA)

Performed detailed analysis on:

### Numerical Features

* Tenure Months
* Monthly Charges
* Total Charges

### Categorical Features

* Contract Type
* Internet Service
* Payment Method
* Technical Support

### Visualizations

* Histograms
* Boxplots
* Countplots
* Correlation Analysis

Key insights were obtained by comparing customer behavior across churn and non-churn groups.

---

## Data Preprocessing

The following preprocessing steps were performed:

* Converted Total Charges to numeric format.
* Handled missing values.
* Removed irrelevant columns.
* Applied One-Hot Encoding on categorical features.
* Prepared feature matrix and target variable.
* Split data into training and testing datasets.

---

## Machine Learning Model

### Random Forest Classifier

A Random Forest Classification model was developed to predict customer churn.

Model training included:

* Train-Test Split
* Random Forest Classification
* Class Imbalance Handling using class_weight='balanced'

---

## Model Evaluation

The model was evaluated using:

* Accuracy Score
* Precision Score
* Recall Score
* F1 Score
* Confusion Matrix
* Classification Report

---

## Hyperparameter Tuning

Different combinations of:

* Number of Trees (n_estimators)
* Maximum Tree Depth (max_depth)

were tested to improve model performance.

The final optimized model used:

* n_estimators = 300
* max_depth = 10
* class_weight = balanced

---

## Feature Importance Analysis

Feature importance was extracted from the Random Forest model to identify the most influential variables affecting customer churn.

Feature selection was also performed by removing low-importance features and retraining the model.

---

## Cross Validation

To evaluate model stability and generalization:

* 5-Fold Cross Validation was performed.
* Accuracy and Recall scores were analyzed across folds.

---

## ROC-AUC Analysis

The model was further evaluated using:

* ROC Curve
* AUC Score

to measure classification performance and discrimination capability.

---

## Customer Segmentation

After churn prediction, customer segmentation was performed using K-Means Clustering.

### Features Used

* Tenure Months
* Monthly Charges
* Total Charges
* Churn Probability

### Steps Performed

* Standardization using StandardScaler
* Elbow Method for optimal cluster selection
* K-Means Clustering

---

## Customer Segments Identified

### Budget Loyal Customers

* Lower spending customers
* Long-term customers
* Low churn probability

### High Risk New Customers

* Short tenure customers
* Higher churn probability
* Potential churn risk

### Loyal Premium Customers

* High-value customers
* Long tenure
* High revenue contribution

---

## Business Insights

* Customers with month-to-month contracts are more likely to churn.
* Higher monthly charges are associated with increased churn probability.
* Technical support services contribute to customer retention.
* Long-tenure customers are generally more loyal.
* Customer segmentation helps businesses target retention campaigns more effectively.

---

## Future Improvements

* Implement XGBoost and LightGBM models.
* Deploy the model using Streamlit.
* Build an interactive dashboard for churn monitoring.
* Develop a real-time churn prediction system.

---
