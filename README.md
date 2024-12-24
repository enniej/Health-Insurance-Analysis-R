# Health-Insurance-Analysis-R
This repository provides statistical analysis and visualisation of health insurance charges using R. It explores key factors like age, BMI, smoking status, and region through regression models, non-parametric tests, and visualisations, offering actionable insights to improve affordability, accessibility, and equity in healthcare coverage.
![image](https://github.com/user-attachments/assets/92d5c9d0-57d5-45eb-adb0-1ca4c2f4108d)
# Health Insurance Charge Analysis Using R

This repository provides an in-depth statistical analysis of health insurance charges. Using regression models, non-parametric tests, and data visualisations, the project explores the effects of factors such as age, BMI, smoking status, and geographical region on health insurance premiums. The findings aim to assist policymakers, insurers, and healthcare stakeholders in improving affordability, accessibility, and equity in healthcare coverage.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Background](#background)
3. [Data Collection and Processing](#data-collection-and-processing)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Methodology](#methodology)
6. [Results](#results)
7. [Recommendations](#recommendations)
8. [Future Work](#future-work)
9. [Conclusion](#conclusion)

---

## 1. Introduction
Health insurance premiums play a crucial role in ensuring access to healthcare services. However, these premiums vary significantly based on demographic, lifestyle, and regional factors. This project utilises statistical tools and predictive modelling in R to analyse and identify the determinants of insurance charges. The goal is to provide actionable insights that support equitable healthcare policies and improve cost efficiency.

---

## 2. Background
Healthcare affordability is a pressing global issue, with insurance premiums often acting as a barrier to accessibility. This project was initiated to investigate the drivers of health insurance charges. By understanding the relationships between personal attributes (e.g., age, BMI, and smoking habits) and charges, the project highlights areas for policy improvements and encourages health-conscious behaviours among individuals.

---

## 3. Data Collection and Processing
### Data Description
The dataset, `Health-Insurance-Dataset.csv`, contains 1,338 records with the following attributes:
- **Numerical Variables**:
  - `age`: Age of the individual.
  - `bmi`: Body Mass Index (BMI).
  - `children`: Number of dependents covered by the insurance.
  - `charges`: Annual insurance premiums in USD.
- **Categorical Variables**:
  - `sex`: Gender (`male`, `female`).
  - `smoker`: Smoking status (`yes`, `no`).
  - `region`: Residential region (`northeast`, `northwest`, `southeast`, `southwest`).

### Data Preprocessing
- **Cleaning**: Checked for missing or inconsistent values and removed duplicates.
- **Encoding**: Converted categorical variables (`sex`, `smoker`, `region`) into factors for analysis.
- **Scaling**: Normalised numerical variables where necessary for regression analysis.
- **Exploration**: Ensured data distributions aligned with real-world expectations before modelling.

---

## 4. Exploratory Data Analysis (EDA)
Key insights derived from the EDA:
- **Age**: Older individuals generally incur higher charges due to increased health risks.
- **BMI**: Higher BMI levels are associated with higher premiums, reflecting potential health risks.
- **Smoking**: Smokers face substantially higher charges, indicating the impact of lifestyle on premium costs.
- **Region**: Geographic disparities in charges suggest differences in regional healthcare accessibility.

Visualisations include:
- Histograms and density plots for numerical variables (`age`, `bmi`, `charges`).
- Bar plots for categorical variables (`smoker`, `region`).
- Correlation matrices and scatter plots illustrating relationships between variables.

**Note**: Visualisations are available in the accompanying report document.

---

## 5. Methodology
### Analytical Techniques
1. **Descriptive Statistics**:
   - Summarised data using mean, median, standard deviation, and skewness for numerical variables.
   - Generated frequency tables for categorical variables.

2. **Statistical Tests**:
   - **Chi-square tests** for independence between categorical variables.
   - **Kruskal-Wallis and Wilcoxon tests** for non-parametric group comparisons.

3. **Regression Analysis**:
   - **Linear Regression**: Explored the relationship between `charges` and all independent variables.
   - **Model Performance**:
     - Adjusted R-squared: Quantified the model's explanatory power.
     - Residual analysis: Verified assumptions of linearity and homoscedasticity.

### Model Variables
- **Dependent Variable**: `charges` (insurance premiums).
- **Independent Variables**: `age`, `bmi`, `children`, `sex`, `smoker`, `region`.

---

## 6. Results
The analysis revealed the following key findings:
1. **Smoking**: Smokers pay significantly higher premiums, with charges nearly doubling on average compared to non-smokers.
2. **BMI**: A strong positive correlation exists between BMI and charges, highlighting potential health risks.
3. **Age**: Insurance charges increase progressively with age, reflecting the rising likelihood of medical expenses.
4. **Region**: Charges vary by region, with the northeast generally having the highest premiums.

Regression analysis indicated:
- Smoking status, BMI, and age were the most significant predictors of insurance charges.
- Adjusted R-squared: 0.75, demonstrating the model's strong predictive ability.

---

## 7. Recommendations
Based on the findings, the following recommendations are proposed:
1. **Policy Design**:
   - Tailor premiums to reward health-conscious behaviours (e.g., maintaining a healthy BMI, quitting smoking).
2. **Geographical Adjustments**:
   - Address regional disparities by investigating underlying healthcare cost drivers.
3. **Customer Engagement**:
   - Provide educational resources to encourage healthier lifestyles, potentially reducing insurance costs.

---

## 8. Future Work
Potential areas for expansion include:
1. **Data Integration**:
   - Incorporating additional data sources, such as medical history and healthcare claims.
2. **Advanced Modelling**:
   - Exploring machine learning algorithms like random forests or gradient boosting for improved predictions.
3. **Dynamic Pricing**:
   - Developing real-time models that adjust premiums based on current health metrics and behaviours.

---

## 9. Conclusion
This project highlights the multifaceted factors influencing health insurance premiums. By leveraging data analytics and statistical modelling, the analysis provides actionable insights to policymakers and insurers. These insights can guide equitable and data-driven policy decisions, promoting healthier behaviours and more affordable healthcare coverage for all.

---


