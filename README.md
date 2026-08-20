# Zenith - A Real Estate Price Predictor

## Overview

Zenith Real Estate Price Predictor is an end-to-end machine learning project that predicts residential property prices using the Ames Housing Dataset. The project leverages exploratory data analysis, feature engineering, data preprocessing, model comparison, hyperparameter tuning, and SHAP-based explainability to build an accurate and interpretable housing valuation system.

The objective is to assist buyers, sellers, investors, and real estate agencies in estimating fair market prices and understanding the factors that influence property values.

---

## Dataset Information

This project uses the Ames Housing Dataset, a comprehensive real-world housing dataset containing detailed information about residential properties sold in Ames, Iowa.

### Dataset Summary

* Records: 2,930 Residential Properties
* Features: 80+ Housing Attributes
* Target Variable: SalePrice
* Problem Type: Supervised Regression
* Missing Values: Present in multiple features and handled during preprocessing

### Target Variable

**SalePrice** – Final sale price of the property in US Dollars.

### Key Feature Categories

* Property Characteristics (Lot Area, Overall Quality, Overall Condition)
* Living Space Features (Above Ground Living Area, Basement Area)
* Garage Information (Garage Area, Garage Capacity)
* Building Age and Remodeling Information
* Neighborhood and Location Features
* Exterior and Interior Quality Indicators

---

## Project Workflow

1. Data Collection and Understanding
2. Exploratory Data Analysis (EDA)
3. Data Cleaning and Missing Value Handling
4. Feature Engineering
5. Data Preprocessing
6. Model Training and Comparison
7. Hyperparameter Tuning
8. Model Evaluation
9. Feature Importance Analysis
10. Model Serialization
11. Model Serialization

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* SHAP
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

## Model Performance

| Model             |          MAE |         RMSE |     R² |
| ----------------- | -----------: | -----------: | -----: |
| XGBoost           | 14819.559570 | 22893.428227 | 0.9346 |
| Gradient Boosting | 14870.180768 | 23243.263087 | 0.9326 |
| Random Forest     | 15883.580478 | 25828.207230 | 0.9167 |
| Linear Regression | 16121.411931 | 29822.510521 | 0.8890 |

### Best Performing Model

**XGBoost** achieved the best overall performance, with the lowest RMSE and the highest R² score among the evaluated models.

---

## Feature Engineering

Custom features were created to improve predictive performance, including:

* House Age
* Remodel Age
* Total Bathrooms
* Total Living Area
* Combined Property Quality Indicators

Feature engineering helped capture additional relationships between housing characteristics and sale prices.

---
## Model Explainability with SHAP

To make the model's predictions interpretable, SHAP (SHapley Additive exPlanations) was applied to the final tuned XGBoost model:

* **Global explainability** — a SHAP summary plot ranks which features most influence predicted prices across the entire test set, and shows whether high or low values push prices up or down.

* **Global explainability** — a SHAP summary plot ranks which features most influence predicted prices across the entire test set, and shows whether high or low values push prices up or down.

This moves the project beyond a black-box predictor, allowing users to understand why a given valuation was produced.

---

## Key Insights

* Overall Quality is one of the strongest predictors of housing prices.
* Living Area and Basement Size significantly impact property valuation.
* Garage Capacity and Garage Area positively influence sale prices.
* Recently remodeled properties generally command higher market values.
* Ensemble-based models outperformed traditional regression approaches.
* XGBoost achieved the best predictive performance among all evaluated models.

---

## Future Improvements

* Deploy the model using Streamlit.
* Incorporate geospatial and neighborhood-level analytics.
* Build a REST API for real-time predictions.
* Integrate current housing market trends and economic indicators.
  
---

## Repository Structure

```text
Zenith-Real-Estate-Price-Predictor/
│
├── data/
│   └── AmesHousing.csv
│
├── notebooks/
│   └── Zenith_Real_Estate_Predictor.ipynb
│
├── models/
│   └── zenith_price_predictor.pkl
│
└── README.md
```

## Author

**Mehak Arora**
