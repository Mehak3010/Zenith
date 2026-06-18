# Zenith- A Real Estate Price Predictor

## Overview

Zenith Real Estate Price Predictor is a machine learning project focused on predicting residential property prices using housing characteristics and socio-economic indicators. The project applies data preprocessing, exploratory data analysis, feature engineering, model training, hyperparameter tuning, and model evaluation techniques to develop an accurate housing price prediction system.

The objective is to help buyers, sellers, investors, and real estate agencies make informed decisions by estimating property values based on key housing attributes.

---

## Dataset Information

The project uses the Boston Housing Dataset, a widely used regression dataset containing information collected by the U.S. Census Service concerning housing in Boston suburbs.

### Dataset Summary

* Records: 506
* Features: 13 Predictor Variables
* Target Variable: MEDV (Median Value of Owner-Occupied Homes)
* Missing Values: None
* Problem Type: Regression

### Feature Description

| Feature | Description                                                         |
| ------- | ------------------------------------------------------------------- |
| CRIM    | Per capita crime rate by town                                       |
| ZN      | Proportion of residential land zoned for lots over 25,000 sq.ft.    |
| INDUS   | Proportion of non-retail business acres per town                    |
| CHAS    | Charles River dummy variable (1 if tract bounds river, 0 otherwise) |
| NOX     | Nitric oxide concentration (parts per 10 million)                   |
| RM      | Average number of rooms per dwelling                                |
| AGE     | Proportion of owner-occupied units built prior to 1940              |
| DIS     | Weighted distances to five Boston employment centres                |
| RAD     | Index of accessibility to radial highways                           |
| TAX     | Full-value property tax rate per $10,000                            |
| PTRATIO | Pupil-teacher ratio by town                                         |
| B       | Population proportion index                                         |
| LSTAT   | Percentage of lower status population                               |
| MEDV    | Median value of owner-occupied homes in $1000s (Target Variable)    |

---

## Project Workflow

1. Data Collection and Understanding
2. Exploratory Data Analysis (EDA)
3. Data Cleaning and Validation
4. Feature Engineering
5. Data Preprocessing
6. Model Training
7. Hyperparameter Tuning
8. Model Evaluation
9. Feature Importance Analysis
10. Model Serialization and Deployment Preparation

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Joblib

---

## Machine Learning Models

The following regression models were evaluated:

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor
* XGBoost Regressor

Model performance was compared using:

* R² Score
* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)

---

## Key Insights

* Average number of rooms (RM) has a strong positive relationship with house prices.
* Lower status population percentage (LSTAT) negatively impacts property value.
* Crime rate and taxation levels influence housing prices.
* Ensemble-based models outperform traditional regression approaches.
* XGBoost achieved the best predictive performance among the evaluated models.

---

## Future Improvements

* Integrate real-time housing market data.
* Deploy the model using Streamlit.
* Implement Explainable AI using SHAP.
* Add geospatial and neighborhood-based features.
* Build a REST API for real-time predictions.
