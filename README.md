# credit-EDA
Home Credit Default Risk - Exploratory Data Analysis (EDA) 
A comprehensive Exploratory Data Analysis (EDA) of the Home Credit Default Risk dataset. This project involves data cleaning, handling missing values, feature engineering, and visualizing key trends to understand the factors influencing loan repayment capabilities.

This repository contains a detailed Exploratory Data Analysis (EDA) performed on the Home Credit Default Risk dataset. The primary goal of this analysis is to identify patterns and insights that distinguish between clients who have difficulties repaying their loans and those who do not.

Project Overview
Loan providers often struggle to lend to people with little or no credit history. Home Credit strives to broaden financial inclusion for the unbanked population by providing a safe positive borrowing experience. This project explores the application data to uncover meaningful correlations between applicant profiles and their repayment history.

Key Features of the Analysis
The notebook follows a systematic data science workflow:
Data Loading & Inspection: Initial look at the application_data.csv comprising 307,511 entries and 122 columns.  
Data Cleaning:
Identified and removed columns with more than 47% missing values to ensure data quality.  
Imputed categorical missing values (like OCCUPATION_TYPE) with "Others".  
Handled numerical missing values (like EXT_SOURCE_3) using median imputation.  
Feature Engineering:
Converted negative time-based columns (Days Birth, Days Employed) into absolute years for better readability.  
Created categorical bins for AMT_CREDIT and AGE_Category to facilitate segmented analysis.  
Data Visualization:
Target Distribution: Analyzed the imbalance in the target variable, finding that approximately 1 in 10 applicants are defaulters.  
Demographic Analysis: Visualized distributions of gender, age groups, and income types.  
Credit Analysis: Examined the distribution of credit amounts across different categories.

Key Insights
Imbalanced Data: About 8.07% of the applicants in the dataset are defaulters.  
Age Demographics: The majority of loan applicants (~50%) fall within the 25-45 age group.  
Gender Split: Female applicants significantly outnumber male applicants, making up approximately 65.8% of the dataset.  
Loan Types: Cash loans are much more common (90.5%) compared to Revolving loans.  
Credit Trends: Most loans are either for relatively low amounts (2-4 lakhs) or very high amounts (8 lakhs+).

Technologies Used
Python
Pandas: Data manipulation and cleaning
NumPy: Numerical operations
Matplotlib & Seaborn: Data visualization and statistical plotting

How to Use
Clone the repository.
Ensure you have application_data.csv in the root directory.
Install dependencies: pip install pandas numpy matplotlib seaborn.
Run the Jupyter Notebook to view the analysis and plots.
