#  :chart_with_upwards_trend: House premiums predictions

This project focuses on predicting house insurance premiums based on some premises attributes using a Machine Learning model

## 📌 Project Overview

**Objective:** Build a predictive model for insurance premium amounts.

**Approach:**
- STEP 1: Exploratory Data Analysis (EDA)
- STEP 2: Data Engineering
- STEP 3: Model Training & Performance Evaluation

## 📊 Data Description

**Numerical data**

- PREMISES_BATHROOMS                    (number of bathrooms of the property)
- PREMISES_BEDROOMS                     (number of bedrooms of the property)
- PREMISES_REBUILD_COST                 (How much it costs to re-build the property)
- PREMISES_YEARS_RESIDENCY              (number of years lived in the property)
- PREMISES_YEAR_BUILT                   (when the premise was built)
- PREMISES_LISTED_IND                   int64
- POTENTIAL_PREMIUM                     (modeled insurance premium)
- MARKET_PREMIUM                        (market insurance premium)

**Categorical data**
- PREMISES_ADDRESS                     (Address of the premise)
- PREMISES_RISK_CODE                   (Post code of the premise)
- PREMISES_PROPERTY_TYPE               (property type)
- PREMISES_NEIGHBOURHOOD_WATCH_IND     (part of a Neighbourhood Watch scheme)

## 🔍 Exploratory Data Analysis (EDA)

 - Data Distribution: Examine the skewness of features.
 - Correlation Analysis: Check if there is a correlation between features.
 - Missing Values: Check for missing values in features


## ⚙️ Feature Engineering
- Create new features that can potentially improve the predictions


## 🤖 Machine Learning Model

Models Used: XGBoost 🚀

- Tree-based gradient boosting model.
- It handles missing values internally


## 📏 Model Performance Evaluation

The performance of the model is evaluated based on the following metrics:
- **Mean absolute error (MAE):** This is the difference between actual and predicted values.  We get an overall idea of how far off the model is
- **Root Mean Squared Error (RMSE)** This is similar to MAE but it penalizes large error more heavily. RMSE is very important because if we have large pricing errors , that's a big financial risk
- **R^2** It measures how well we capture premium variation. The closer to 1 the better our predictions
- **Mean Absolute Percentage Error (MAPE)** It mesures relative error (%) compared to absolute error (£). It highlights big errors in predictions
