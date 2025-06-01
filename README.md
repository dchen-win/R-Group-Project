
# Group project 1:
📈 Data Analysis: Income, Education, Occupation & Demographics  
Authors: 
- Cindy Chen
- Mai Castellano
- Tyler Kussee
- Spencer Hutchison  
Date: Spring 2025

📄 Overview  
This project analyzes 2022 Oregon PUMA microdata to investigate relationships between household income and demographic factors such as education, occupation, race/ethnicity, homeownership, and marital status. Using exploratory data analysis and linear regression modeling, the study identifies key predictors of income and occupation.

🎯 Objectives  
- Explore income distributions by race, education, and occupation  
- Understand occupation patterns across homeownership and marital status  
- Build regression models to predict income and occupation groups  
- Evaluate interaction effects among demographic variables  

🧾 Dataset Description  
The dataset includes 2022 Public Use Microdata Area (PUMA) survey data for Oregon:  
- `Income`: Household income (filtered for non-zero)  
- `EducationGroup`: Categorized education levels  
- `OccupationGroup`: Broad occupation categories  
- `Race`: Self-reported race/ethnicity  
- `HomeOwnership`: Homeownership status  
- `MaritalStatus`: Marital status categories  

Data preparation involved filtering adults (age ≥14), transforming categorical variables, and cleaning income values.

🔍 Methodology  
1. **Data Exploration**  
   - Visualized income distributions by race and occupation groups using histograms  
   - Examined occupation distributions across homeownership and marital status  

2. **Regression Modeling**  
   - Fit linear models predicting income and occupation based on education, race, homeownership, and marital status  
   - Tested interaction terms between occupation and homeownership, marital status, and race  
   - Compared models via ANOVA for improved fit  
   - Assessed model diagnostics including residual plots and QQ-plots  

📊 Visualizations  
- Income histograms split by race and occupation reveal income disparities  
- Bar plots show occupation distribution differences by homeownership and race  
- Diagnostic plots highlight model fit and areas for improvement  

📦 Tools & Libraries  
R packages used:  
- `tidycensus` for data retrieval  
- `tidyverse` (dplyr, ggplot2) for data wrangling and visualization  
- Base `lm()` for regression modeling  

---

# Group Project 2: 
🚗 Vehicle Loan Default Prediction  
**Authors:**  
Di Chen  
Mai Castellano  
Tyler Kussee  
Spencer Hutchison  

**Date:** Spring 2025

## 📄 Overview  
This project focuses on analyzing and modeling vehicle loan default using a comprehensive dataset with approximately 41 features. The dataset contains borrower details (such as date of birth, employment type, and credit score) and loan specifics (like disbursal amount and loan-to-value ratios). The main goal is to identify key predictors of loan default and develop a classification model to accurately predict defaults.

## 🎯 Objectives  
- Clean and preprocess raw vehicle loan data, handling complex date/time fields and missing values  
- Identify the most influential explanatory variables driving loan default  
- Develop and evaluate predictive models, focusing on XGBoost and logistic regression classifiers  
- Interpret model results and assess feature importance to understand loan default drivers  

## 🧾 Dataset Description  
The dataset was sourced from Kaggle’s Vehicle Loan Default Prediction challenge, featuring:  
- Loan applicant details: Date of birth, employment type, credit history length, credit score  
- Loan information: Loan disbursal amount, loan-to-value (LTV) ratio, loan status (default/non-default)  
- Approximately 41 columns with one binary response variable indicating loan default status  

Data preprocessing included date conversions, creating dummy variables for employment types, handling missing values, and removing duplicates.

## 🔍 Methodology  

### Data Cleaning & Feature Engineering  
- Standardized age and account length variables from date and string formats  
- Created dummy variables for employment categories  
- Removed rows with missing or duplicate values  

### Exploratory Analysis  
- Computed correlation matrix to examine relationships among variables  
- Identified top 10 important features using XGBoost feature importance scores  

### Modeling  
- Trained an XGBoost classifier with cross-validation to optimize training rounds  
- Selected key features based on importance scores for further modeling  
- Built logistic regression model on top features and evaluated accuracy, precision, and recall  

## 📊 Visualizations  
- Feature importance plot highlighting top predictors of loan default  
- Heatmap of correlation matrix to visualize relationships between variables  
- Confusion matrix and model evaluation metrics for logistic regression classifier  

## 📦 Tools & Libraries  
- **R packages:** tidycensus, tidyverse (dplyr, ggplot2), caret, xgboost  
- Data manipulation and visualization with tidyverse  
- Machine learning with xgboost and caret  
- Logistic regression using base glm() function  

