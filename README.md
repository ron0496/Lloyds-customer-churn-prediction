# Lloyds-customer-churn-prediction

This internship is provided by [Forage](https://www.theforage.com/simulations/lloyds-banking-group/data-science-fpey)

This repository contains the [code and resources]() for the Data Science & Analytics Internship Program at Lloyds Banking Group through Forage . This program was divided into 3 tasks, each of which was designed to give me a taste of the work that data scientists and analysts do at Lloyds Banking Group. The tasks involved analyzing customer data, building predictive models, and presenting findings to stakeholders.The tasks were as follows:

1. Intro & Scenario

2. Task 1: Data gathering and exploratory analysis

3. Task 2: Building a machine learning model

## Intro & Scenario
As a recent data science graduate, I'm eager to apply my skills to predict customer churn and contribute to a meaningful impact here at Lloyds Banking Group.

My initial goals for this phase are to:

* Collaborate closely with the team to understand the available data sources relevant to customer behaviour and churn.

* Begin the process of exploratory data analysis to identify initial patterns, trends, and potential relationships within the data.

* Familiarize myself with the data cleaning and preprocessing steps required to ensure data quality for model building.

* Start researching suitable predictive modelling techniques that can be applied to customer churn prediction.

* Consider potential evaluation metrics that can effectively measure the performance of the churn prediction model.

## Task 1: Data gathering and exploratory analysis

Relevant data was gathered from multiple sources, including Customer_Demographics, Transaction_History, Customer_Service, Online_Activity, and Churn_Status, to explore factors contributing to customer churn.

The selection process prioritized data that offered meaningful insights into customer profiles, purchasing behavior, service interactions, online activity, and churn outcomes.

Exploratory Data Analysis (EDA) was performed using visual tools such as:
	•	Histograms to show distributions of age, spending, and login frequency by churn status
	•	A heatmap to visualize the relationship between age and amount spent, revealing churn clusters
	•	Count plots to compare churn rates across gender, income levels, and service usage

Descriptive statistics were calculated for features such as gender, age, marital status, income level, amount spent, product category, interaction type, resolution status, login frequency, and service usage to understand the structure and trends in the data.

Missing values were identified in DaysSinceLastInteraction, InteractionType, and ResolutionStatus and documented for future handling.

Numerical features including Age, IncomeLevel, Total_amount_spent, Transaction_frequency, DaysSinceLastInteraction, LoginFrequency, and DaysSinceLastLogin were standardized using the scale function in base R to ensure consistent scaling for modeling.

Categorical variables like Gender, MaritalStatus, IncomeLevel, ProductCategory, InteractionType, ResolutionStatus, and ServiceUsage were encoded using one-hot encoding and label encoding to convert them into a machine-readable format.

All datasets were merged into a final consolidated dataframe, customer_churn_df, using CustomerID as the key.

A final report was compiled outlining the data collection, EDA insights with visualizations, descriptive analysis, and the preprocessing steps performed, resulting in a clean and structured dataset ready for modeling.

Resources: [Task 1 Report](https://github.com/ron0496/Lloyds-customer-churn-prediction/blob/main/Task%201.pdf)

## Task 2: Building a machine learning model

Chosen XGBoost (Extreme Gradient Boosting) as the machine learning algorithm for predicting customer churn due to its strong predictive performance and ability to capture complex, non-linear patterns. It handles class imbalance and missing values effectively, which are common in churn datasets. Moreover, it provides feature importance metrics that enhance model interpretability and support business decisions.

Preprocessing involved loading and merging relevant datasets, removing irrelevant columns, separating features from the target variable (ChurnStatus), identifying categorical and numerical variables, and applying tailored preprocessing pipelines: imputation and one-hot encoding for categorical features, and imputation with standardization for numerical ones. The data was then split into training and testing sets using sample.split().

Trained an XGBoost model using the preprocessed training data.

Assessed model performance on the test set using several metrics: Classification report, ROC-AUC score (0.56) to measure the model’s ability to distinguish between classes, Sensitivity (Recall / True Positive Rate at 63%) to evaluate how well churners were identified, and Specificity (True Negative Rate at 59%) to measure correct identification of non-churners. The Confusion Matrix provided a visual representation of true/false positives and negatives, with an overall accuracy of 60%, indicating moderate predictive capability.

To understand which factors contributed most to churn prediction, we analyzed the top 10 most important features using the trained XGBoost model. The features with the highest influence were:
Total_amount_spent, Age, DaysSinceLastInteraction, LoginFrequency, DaysSinceLastLogin, Transaction_frequency, Groceries, Books, IncomeLevel, and ServiceUsage_Website.

Generated business recommendations based on model predictions, such as initiating targeted retention campaigns for high-risk customers, implementing churn prevention strategies by addressing root causes, using churn risk scores for customer segmentation and personalization, and optimizing resource allocation by prioritizing valuable at-risk customers.

Outlined improvement opportunities, including advanced feature engineering, evaluating simpler models for faster deployment, setting up regular retraining with updated data, integrating feedback from retention initiatives, and performing cost-benefit analysis of various retention tactics.

Prepared a detailed report covering the reasoning behind algorithm selection, data preprocessing steps, model development and evaluation, actionable business insights, and suggestions for future enhancements.

Resources: [Task 2 Report](https://github.com/ron0496/Lloyds-customer-churn-prediction/blob/main/Task%202.pdf)

(Certificate Link)[https://forage-uploads-prod.s3.amazonaws.com/completion-certificates/Zbnc2o4ok6kD2NEXx/EuvC8GPjkZ6xaiP9p_Zbnc2o4ok6kD2NEXx_aXM3Xh4DNSNAw9pzW_1747342336748_completion_certificate.pdf)
