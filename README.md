# Lloyds-customer-churn-prediction

This repository contains the code and resources for the Data Science & Analytics Internship Program at Lloyds Banking Group through Forage. This program was divided into 3 tasks, each of which was designed to give me a taste of the work that data scientists and analysts do at Lloyds Banking Group. The tasks involved analyzing customer data, building predictive models, and presenting findings to stakeholders.The tasks were as follows:

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
