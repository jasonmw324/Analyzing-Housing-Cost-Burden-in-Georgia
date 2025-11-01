# 🏘️ Analyzing Housing Cost Burden in Georgia

This analysis examines the factors that contribute to the percentage of housing in Georgia that is considered cost-burdened, and explores relationships between income, household characteristics, and location.


## 🧭 Overview
This project investigates housing cost burden in Georgia, defined as households spending more than 30% of income on housing. The goal is to identify key demographic, economic, and geographic factors associated with cost-burdened households and provide insights for policymakers and housing researchers.

---

## 🛠️ Skills & Tools Used
- Programming: R
- Libraries: tidyverse, dplyr, tidycensus 
- Statistical Analysis: Multiple Linear Regression, Welch's Anova, Weighted Least Squares

---

## 🎯 Research Question
- What is the relationship between demographic, geographic, and
economic features collected by the Census Bureau’s American
Community Survey on the percentage of owner- and renter-occupied
housing that is classified as cost-burdened (e.g., 30% of their income
dedicated to housing costs)?  
  

---

## 📊 Data Source
- **Dataset name:** American Community Survey (ACS) 5-year estimates 2017-2021
- **Source/Link:** [ACS Data via Census API](https://www.census.gov/programs-surveys/acs)   
- **Number of observations / variables:** Varies by table; includes household income, rent, household size, and county-level identifiers  
- **Any preprocessing notes:** Filtered for Georgia; calculated rent-to-income ratio; handled missing income and rent data  

---

## 🧹 Data Preparation
- Removed records with missing or zero income or rent  
- Filtered for Georgia households only  
- Created new variable: rent-to-income ratio  
- Aggregated data to county level for certain analyses  
- Checked for outliers and extreme values in income and rent  

---

## ⚙️ Methodology
- Multiple Linear Regression
- Weighted Least Squares
- Welch's ANOVA   

---

---

## 📈 Results & Conclusions
- Urban vs. Rural: Urban counties show a significantly higher percentage of renter-occupied cost-burdened households (+9.43%) compared to rural areas.
- Income Effects: Increases in median household income are correlated with lower cost burden for renters—but the impact is modest.
- Education Paradox: Counties with higher percentages of bachelor’s degrees unexpectedly see slightly higher rates of cost-burdened households for renter-occupied
households.
- Age disparities
  - Owners: The youngest (15–24) and oldest (65+) homeowners face notably higher cost burdens than middle-aged groups.
  - Renters: Older adults (65+) are significantly more likely to be cost-burdened compared to younger renters.
- Racial Inequities
  - Owners: Black and “Other” racial groups have higher owner cost-burden rates than White owners.
  - Renters:Black renters experience significantly higher cost burden compared to White and Other groups. 

---








