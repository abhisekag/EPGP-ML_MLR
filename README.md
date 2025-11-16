**BoomBikes Demand Prediction: Multiple Linear Regression**

This project focuses on building a robust Multiple Linear Regression model to identify the key factors driving bike rental demand for the bike-sharing company, BoomBikes, and to accurately predict future rental counts.

**Table of Contents**

**General Info

Technologies Used

Conclusions

Contact**


**General Information**

Project Background: BoomBikes, a US-based bike-sharing company, needs a clear understanding of the market dynamics to plan their business operations, inventory, and marketing strategies effectively.

Business Problem: To model the relationship between bike demand (total rental count, cnt) and various independent variables (weather, season, holidays, etc.) to help management predict demand and identify key controllable factors.

Dataset Used: The day.csv file, which contains daily bike rental data, along with environmental and calendar variables, collected over a two-year period (2018-2019).

**Conclusions**

The final model was built using an iterative process of feature selection based on P-values and Variance Inflation Factor (VIF) checks, resulting in a strong and interpretable model:

High Predictive Power: The final model achieved an R^2 score of approximately 0.82 on the test data, indicating that the selected features explain about 82% of the variance in the bike rental demand.

Top Positive Predictors: The most significant positive factors driving demand are Year (yr) and Feeling Temperature (atemp). The yr=1 coefficient is one of the highest, indicating a substantial, permanent growth in bike-sharing popularity from 2018 to 2019.

Negative Impact of Season/Weather: The demand is significantly lower during the Spring season (season_spring) and under the worst modeled weather condition, Light Rain/Snow (weathersit_LightRain_Snow).

Strategic Insight: The company should prioritize maintenance and operational capacity during peak periods (Summer and Fall) and capitalize on the sustained year-over-year growth identified by the yr variable.

**Technologies Used**

Python
Pandas: For data manipulation and cleaning.
NumPy: For numerical operations.
Matplotlib & Seaborn: For exploratory data analysis and residual analysis visualization.
Scikit-learn (sklearn): For data splitting (train_test_split) and scaling (MinMaxScaler).
Statsmodels: For Ordinary Least Squares (OLS) model training, statistical summary, and VIF calculation.

**Contact**
Created by [@abhisekag] - feel free to contact me!
