# Zenith - A Real Estate Price Predictor

## Overview

Zenith Real Estate Price Predictor is an end-to-end machine learning project that predicts residential property prices using the Ames Housing Dataset. The project leverages exploratory data analysis, feature engineering, data preprocessing, model comparison, and hyperparameter tuning to build an accurate and interpretable housing valuation system.

The objective is to assist buyers, sellers, investors, and real estate agencies in estimating fair market prices and understanding the factors that influence property values.

---

## Dataset Information

This project uses the Ames Housing Dataset, a comprehensive real-world housing dataset containing detailed information about residential properties sold in Ames, Iowa.

Unlike traditional housing datasets, Ames Housing includes a rich set of structural, neighborhood, quality, and property-related features, making it ideal for advanced regression modeling and predictive analytics.

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

## Feature Engineering

Custom features were created to improve predictive performance, including:

* House Age
* Remodel Age
* Total Bathrooms
* Total Living Area
* Combined Property Quality Indicators

Feature engineering helped capture additional relationships between housing characteristics and sale prices.

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
* Add Explainable AI using SHAP.
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
├── README.md
│
└── requirements.txt
```

## Author

**Mehak Arora**
