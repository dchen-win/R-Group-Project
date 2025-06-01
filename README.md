---
title: "README: PUMA Data Analysis"
output: github_document
---
Group project 1:
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

