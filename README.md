# Project Report: Customer Churn Analysis

## Introduction

This report presents an analysis of customer churn data, with the goal of understanding the factors that influence customer retention and developing predictive models to identify customers at risk of churning. The data source for this project is `customer-churn.csv`, and the code used for the analysis is provided in both PDF (`customer-churn.pdf`) and CSV (`customer-churn.csv`) formats.

## Data Description

The `customer-churn.csv` file contains information about a telecommunications company's customers, including:

- Customer demographic information (e.g., gender, partner status, dependents)
- Services subscribed (e.g., phone, internet, online security, streaming TV/movies)
- Contract details (e.g., contract type, paperless billing, payment method)
- Account information (e.g., tenure, monthly charges, total charges)
- Churn status (whether the customer has left the company or not)

## Data Manipulation

- Importing necessary libraries (pandas, numpy, matplotlib, plotly)
- Loading the data into a DataFrame
- Extracting specific columns and filtering rows based on conditions
- Handling missing values and data cleaning
- Creating new DataFrames from the original data

## Data Visualization

- Bar plot to show the distribution of internet service types
- Histogram to visualize the distribution of customer tenure
- Scatter plot to explore the relationship between tenure and monthly charges
- Box plot to compare customer tenure across different contract types

## Machine Learning Concepts

- ## Linear Regression
   - Dependent variable: Monthly charges
   - Independent variable: Tenure
   - Splitting the data into training and testing sets
   - Building the model on the training set
   - Predicting values on the testing set
   - Calculating the root mean squared error (RMSE) to evaluate model performance

- ## Logistic Regression
   - Binary classification problem: Predicting customer churn (Yes/No)
   - Dependent variable: Churn
   - Independent variables:
     - Scenario 1: Monthly charges
     - Scenario 2: Tenure and monthly charges
   - Splitting the data into training and testing sets
   - Building the model on the training set
   - Predicting values on the testing set
   - Constructing a confusion matrix
   - Calculating the accuracy score

-  ## Decision Tree
   - Dependent variable: Churn
   - Independent variable: Tenure
   - Splitting the data into training and testing sets
   - Building the decision tree model on the training set
   - Predicting values on the testing set
   - Constructing a confusion matrix
   - Calculating the accuracy score

- ## Random Forest
   - Dependent variable: Churn
   - Independent variables: Tenure and monthly charges
   - Splitting the data into training and testing sets
   - Building the random forest model on the training set
   - Predicting values on the testing set
   - Constructing a confusion matrix
   - Calculating the accuracy score

## Key Findings

Based on the analysis performed in this project, the following are some key findings:

- **Customer Tenure**
   - The distribution of customer tenure shows a significant portion of customers with relatively short tenure (less than 24 months).
   - Customers with longer tenure tend to have higher monthly charges, as indicated by the positive correlation in the scatter plot.

- **Internet Service**
   - A substantial number of customers subscribe to fiber optic internet service, followed by DSL and a smaller portion with no internet service.

- **Contract Type**
   - The box plot reveals that customers with longer-term contracts (one year or two years) generally have a higher tenure compared to those on month-to-month contracts.

- **Linear Regression Model**
   - The linear regression model, with monthly charges as the dependent variable and tenure as the independent variable, achieved a root mean squared error (RMSE) of 29.39.
   - This model provides a baseline understanding of the linear relationship between customer tenure and monthly charges.

- **Logistic Regression Models**
   - The logistic regression model with monthly charges as the sole independent variable achieved an accuracy of around 73% in predicting customer churn.
   - Incorporating both tenure and monthly charges as independent variables improved the accuracy to approximately 79%.
   - The confusion matrix revealed that the model struggled more with identifying potential churners than non-churners.

- **Decision Tree and Random Forest Models**
   - The decision tree model, using tenure as the independent variable, achieved an accuracy of 75% in predicting customer churn.
   - The random forest model, with tenure and monthly charges as independent variables, also achieved an accuracy of 75%.
   - These tree-based models performed reasonably well but did not significantly outperform the logistic regression models for this dataset.

These findings provide insights into the factors influencing customer churn and serve as a basis for further exploration and model refinement. Additional features or data transformations could potentially improve the predictive performance of the models.
## Conclusion

This project showcases various data manipulation, visualization, and machine learning techniques applied to a customer churn dataset. The analysis explores different algorithms, including linear regression, logistic regression, decision trees, and random forests, to predict customer churn based on various features. The report provides a comprehensive understanding of the process, from data preprocessing to model evaluation, using appropriate metrics and visualizations.

