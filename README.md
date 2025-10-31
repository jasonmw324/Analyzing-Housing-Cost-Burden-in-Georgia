# 🏘️ Analyzing Housing Cost Burden in Georgia

This analysis examines the factors that contribute to the percentage of housing in Georgia that is considered cost-burdened, and explores relationships between income, household characteristics, and location.

---

## 📚 Table of Contents
1. [Overview](#overview)
2. [Skills & Tools Used](#skills--tools-used)
3. [Research Question](#research-question)
4. [Data Source](#data-source)
5. [Data Preparation](#data-preparation)
6. [Methodology](#methodology)
7. [Assumptions](#assumptions)
8. [Results](#results)
9. [Visualizations](#visualizations)
10. [Project Structure](#project-structure)
11. [Limitations](#limitations)
12. [Future Work](#future-work)
13. [License](#license)
14. [Acknowledgements](#acknowledgements)

---

## 🧭 Overview
This project investigates housing cost burden in Georgia, defined as households spending more than 30% of income on housing. The goal is to identify key demographic, economic, and geographic factors associated with cost-burdened households and provide insights for policymakers and housing researchers.

---

## 🛠️ Skills & Tools Used
- Programming: R
- Libraries: tidyverse, dplyr, tidycensus 
- Statistical Analysis: Multiple Linear regression, Welch's Anova, Weighted Least Squares

---

## 🎯 Research Question
- What factors contribute most to the prevalence of cost-burdened households in Georgia?  
- How do income, household size, and geographic location relate to housing cost burden?  

---

## 📊 Data Source
- **Dataset name:** American Community Survey (ACS) 5-year estimates  
- **Source/Link:** [ACS Data via Census API](https://www.census.gov/programs-surveys/acs)  
- **Time period covered:** 2015–2020  
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
- Performed descriptive statistics to understand distribution of cost-burdened households  
- Used linear regression to model relationship between demographic variables and cost burden  
- Conducted t-tests and ANOVA to explore differences across counties and income groups  
- Visualized trends with ggplot2 and interactive plots using plotly  

---

## 📏 Assumptions
- ACS survey weights correctly reflect population estimates  
- Linear regression assumptions: linearity, independence, normality of residuals, and homoscedasticity  
- County-level aggregation does not mask significant sub-county variation  

---

## 📈 Results
- Income and household size were the strongest predictors of cost-burdened status  
- Certain counties exhibited significantly higher prevalence of housing cost burden  
- Education level and employment status showed moderate associations with rent-to-income ratio  

---

## 🖼️ Visualizations
```markdown
![Cost Burden by County](images/cost_burden_map.png)
![Rent-to-Income Distribution](images/rent_income_plot.png)




