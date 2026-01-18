# Housing Price Prediction Assignment

A regression analysis project to predict the actual value of prospective properties for Surprise Housing's entry into the Australian market.

## Table of Contents

- [General Information](#general-information)
- [Conclusions](#conclusions)
- [Technologies Used](#technologies-used)


## General Information

### Background
Surprise Housing, a US-based housing company, is planning to expand into the Australian real estate market. They operate by purchasing houses below their actual value and flipping them for a profit.

### Business Problem
The company needs a model to predict the actual value of prospective properties based on various features (like size, location, amenities, etc.). This will help them identify undervalued properties and make informed investment decisions.

### Dataset
The project uses a dataset of house sales in Australia, containing 1460 entries with 81 explanatory variables describing every aspect of residential homes.

## Conclusions

### Model Performance
Regularized regression models proved effective. Lasso Regression was chosen as the final model because it offered a high predictive accuracy ($R^2 \approx 0.86$) while simultaneously performing feature selection, making the model easier to interpret for business stakeholders.

### Key Predictors
The most significant variables driving house prices were identified as:

- Above Grade Living Area (GrLivArea): Larger living areas command higher prices.
- Overall Quality (OverallQual): The material and finish of the house are critical.
- Neighborhood: Specific locations like NoRidge and NridgHt are associated with significantly higher property values.
- Garage Capacity: The size and car capacity of the garage (GarageCars, GarageArea) are strong positive indicators.

### Regularization
The optimal regularization strength (Alpha) was found to be 500 for Ridge and 1000 for Lasso, indicating a need to penalize complexity to prevent overfitting.

## Technologies Used

- Python - version 3.x
- Pandas - version 1.3.x (for data manipulation)
- NumPy - version 1.21.x (for numerical operations)
- Matplotlib - version 3.4.x (for visualization)
- Seaborn - version 0.11.x (for advanced visualization)
- Scikit-learn - version 0.24.x (for machine learning modeling)

## Contact
Created by [@abhisekag] - feel free to contact me!