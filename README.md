# BoomBikes Demand Prediction: Multiple Linear Regression

This project aims to build a robust Multiple Linear Regression (MLR) model to identify the key factors driving bike rental demand for the bike-sharing company, BoomBikes. The goal is to accurately predict future demand and provide strategic insights for business planning.

---

## Table of Contents

1. [General Information](#general-information)
2. [Conclusions](#conclusions)
3. [Technologies Used](#technologies-used)
4. [Contact](#contact)

---

## General Information

**Project Background:**  
BoomBikes, a US-based bike-sharing company, seeks a clear understanding of market dynamics to plan business operations, manage inventory, and develop effective marketing strategies.

**Business Problem:**  
Model the relationship between bike demand (total rental count: `cnt`) and various independent variables such as weather, season, and holidays. This will help management predict demand and identify actionable factors for growth.

**Dataset Used:**  
- **File:** `day.csv`
- **Contains:** Daily bike rental counts along with environmental and calendar variables.
- **Time Period:** Two years (2018-2019)

---

## Conclusions

The final MLR model was developed using an iterative feature selection process based on p-values and Variance Inflation Factor (VIF) analysis, resulting in a strong and interpretable model:

- **High Predictive Power:**  
  The final model achieved an **R² score of approximately 0.82** on the test data, meaning the selected features explain about 82% of the variance in bike rental demand.

- **Top Positive Predictors:**  
  - **Year (`yr`):** The `yr=1` coefficient is among the highest, indicating substantial and persistent growth year-over-year.
  - **Feeling Temperature (`atemp`):** Higher perceived temperature is strongly associated with increased bike rentals.

- **Negative Impact of Season/Weather:**  
  - **Spring (`season_spring`):** Demand drops significantly during the spring season.
  - **Light Rain/Snow (`weathersit_LightRain_Snow`):** Severe weather conditions negatively affect rental counts.

- **Strategic Insight:**  
  BoomBikes should prioritize maintenance and operational capacity during peak seasons (Summer and Fall), and capitalize on the sustained year-over-year growth identified by the `yr` variable.

---

## Technologies Used

- **Python**
- **Pandas:** Data manipulation and cleaning.
- **NumPy:** Numerical operations.
- **Matplotlib & Seaborn:** Visualizations for exploratory data analysis and residual analysis.
- **Scikit-learn:** Data splitting (`train_test_split`), scaling (`MinMaxScaler`).
- **Statsmodels:** Training the Ordinary Least Squares (OLS) model, statistical summaries, VIF calculation.

---

## Contact

Created by [@abhisekag] – feel free to contact me!
