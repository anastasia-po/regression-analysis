# Regression Analysis of Spending Behavior

## Project Overview
The dataset that was used for this analysis contains 1010 rows of individuals’ preferences and demographic characteristics. The primary focus of this analysis is to identify factors that influence individuals’ spending patterns and to develop an accurate predictive model. The main hypothesis is that **women spend more money on appearance than men**. The report demonstrates the results of correlation analysis, simple linear regression, and multiple linear regression.

---

## Dataset Description
- 1,010 respondents
- 150 variables (139 integer and 11 categorical).
- Age: 15–30 years (average 20)
- Country: Slovakia  
- Data source: students and their social circle (university survey)
- All answers are given on a **1–5 Likert scale**

The variables can be split into the following groups:

- Music preferences (19 items)
- Movie preferences (12 items)
- Hobbies & interests (32 items)
- Phobias (10 items)
- Health habits (3 items)
- Personality traits, views on life, & opinions (57 items)
- Spending habits (7 items)
- Demographics (10 items)

---
## Tools & Methods
- Python  
  - pandas  
  - numpy  
  - matplotlib  
  - statsmodels
  - seaborn  

- Correlation Analysis  
- Simple Linear Regression  
- Multiple Linear Regression

---
## Analysis

### 1. Data Preparation
- Filtered rows with missing values
- Encoded gender variable into numeric format (1 — male, 2 — female)

### 2. Correlation Analysis
- Calculated correlation between spending on appearance and gender  
- Found a **weak positive correlation (0.12)**

### 3. Simple Linear Regression
- Built a model using gender as the only predictor
- Results:
  - **R² = 0.015**
  - The effect is statistically significant but weak
  - Gender alone explains only about **1.5% of spending variance**

### 4. Multiple Linear Regression
Added the following predictors:
- Gender  
- Age  
- Shopping interest  
- Socializing interest  

Results:
- **R² increased to 0.276**
- **Shopping interest** became the strongest predictor (positive correlation (0.51))
- Gender and socializing interest showed weak positive effects
- Age was not statistically significant

---

## Key Findings
- Women spend slightly more on appearance than men (**+0.3 points on a 1–5 scale**)  
- Gender alone has **low explanatory power**  
- **Shopping interest is the strongest predictor of spending on appearance**  
- Multiple regression significantly improved model performance (**R² = 0.276**)

---

## Future Improvements
Future work would involve trying to identify stronger predictive variables such as shopping interest to improve the accuracy of the regression model.

---

## Limitations
Limitations included the fact that given conclusions only related to this specific group of people with concrete age and country but can’t be related, for example, to the oldest people in this country. Also, participants can be biased in estimating their personal characteristics.

