# Loan Data Exploration

This project explores and analyzes a loan dataset to uncover insights into the demographics and loan approval patterns of the applicants.

## Project Overview

This analysis covers various aspects of the dataset, including demographic distribution, loan approval rates by different categories, and potential factors influencing loan approval. The project is implemented using R, leveraging libraries like `ggplot2` and `dplyr` for data manipulation and visualization.

## Data Loading and Initial Exploration

- **Loading Data:** The dataset is loaded from a CSV file and the first few rows are previewed.
- **Structure of Data:** The structure of the dataset is examined to understand the types of variables.
- **Summary Statistics:** Summary statistics provide an overview of the central tendency and spread of each variable.
- **Missing Values Handling:** Columns with missing values are identified and handled using appropriate techniques like mean imputation and mode substitution.

## Data Cleaning

- **Handling Missing Values:** 
  - Missing values in `LoanAmount` and `Loan_Amount_Term` are filled with the mean.
  - Missing values in `Credit_History` are filled with the mode.
- **Data Standardization:**
  - Categorical variables like `Loan_Status`, `Gender`, `Married`, `Dependents`, and `Self_Employed` are standardized.
- **Duplicates:** No duplicate records was found.

## Feature Engineering

- **Income Category:** A new column `IncomeCategory` is created to categorize applicants based on their income.

## Data Visualization and Analysis

### Frequency Distribution

- **Gender Distribution:** Visualization of loan applicants by gender.
- **Income Category Distribution:** Distribution of applicants across different income categories.
- **Marital Status Distribution:** Analysis of applicants by marital status.
- **Dependents Distribution:** Distribution of the number of dependents among applicants.
- **Education Distribution:** Analysis of applicants' educational backgrounds.
- **Employment Status Distribution:** Distribution of applicants by employment status.
- **Credit History Distribution:** Visualization of applicants' credit history.
- **Property Area Distribution:** Analysis of applicants by property area.
- **Loan Status:** Visualization of loan approval rates.

### Distribution Analysis

- **Loan Amount by Gender:** Boxplot of loan amounts distributed by gender.
- **Applicant Income by Marital Status:** Boxplot analysis of income distribution by marital status.
- **Correlation:** Scatter plot with a trend line to examine the correlation between applicant income and loan amount.

### Loan Approval Rate Analysis

- **By Gender:** Loan approval rates by gender.
- **By Marital Status:** Loan approval rates by marital status.
- **By Education:** Analysis of loan approval rates by educational background.
- **By Employment Status:** Loan approval rates by employment status.
- **By Property Area:** Loan approval rates by property area.
- **By Income Category:** Analysis of loan approval rates across different income categories.

## Summary of Analysis

- **Demographic Distribution:** Key insights into the distribution of various demographic features.
- **Loan Approval Patterns:** Analysis of how different factors influence loan approval rates.
  
## Insights

- No strong correlation between income and loan amount suggests loan approval is not solely based on income level.
- Graduates have a slightly higher loan approval rate, indicating education may influence approval decisions.
- Consistent loan approval rates across employment status and income categories suggest a uniform approval process.
- Regional variations in loan approval rates could be inferred from the slightly higher approval in Semiurban areas.

## Conclusion

This analysis provides valuable insights into the loan application process, highlighting the influence of demographic and financial factors on loan approval rates. The findings can be leveraged to optimize loan processing strategies and enhance decision-making.

- Data Source: [Kaggle](https://www.kaggle.com/datasets/burak3ergun/loan-data-set?resource=download)
