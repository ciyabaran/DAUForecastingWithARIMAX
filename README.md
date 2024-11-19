
# Project Name: Time Series Analysis with DAU and Daily New User Forecasting

This project uses ARIMA and ARIMAX models to predict daily active users (DAU) and daily new users of a mobile gaming application. The goal is to analyze the session data and forecast user behavior to inform business strategies.

## Table of Contents

- [Project Description](#project-description)
- [Technologies Used](#technologies-used)
- [Data Analysis](#data-analysis)
  - [Data Exploration](#data-exploration)
  - [Data Manipulation](#data-manipulation)
  - [Data Visualization](#data-visualization)
- [Modeling Approach](#modeling-approach)
  - [Stationarity Test with ADF](#stationarity-test-with-adf)
  - [ACF and PACF Analysis](#acf-and-pacf-analysis)
  - [Daily New User Forecasting with ARIMA](#daily-new-user-forecasting-with-arima)
  - [DAU Forecasting with ARIMAX](#dau-forecasting-with-arimax)
- [Results and Insights](#results-and-insights)
- [Contact](#contact)

## Project Description

This project aims to analyze user interactions in a gaming application to forecast daily active users (DAU) and daily new users for the next 30 days. These forecasts are critical for shaping business strategies and marketing campaigns.

## Technologies Used

- **Python**: The primary programming language for this project.
- **Pandas**: Used for data processing and manipulation.
- **NumPy**: Used for numerical computations and array operations.
- **Matplotlib and Seaborn**: Used for data visualization.
- **Statsmodels**: Used for statistical modeling and time series analysis.
- **ARIMA and ARIMAX Models**: Time series forecasting models.
- **Jupyter Notebook**: Used for interactive coding and presenting results.

## Data Analysis

### Data Exploration

- **Data Loading**: Session data and other related datasets were loaded.
- **Preliminary Examination**: Data types, missing values, and general statistics were examined.
- **Null Check**: Missing or erroneous data was identified and cleaned.

### Data Manipulation

- **Daily Active Users (DAU) Calculation**: Daily active user counts were derived from session data.
- **Daily New User Calculation**: The number of new users joining the application each day was calculated.
- **Data Merging**: DAU and daily new user data were combined into a single dataset.

### Data Visualization

- Time series graphs were created for DAU and daily new user counts.
- Trends and seasonality in user behavior were analyzed.

## Modeling Approach

### Stationarity Test with ADF

- **Purpose**: To determine if the time series is stationary.
- **Result**: The p-value of the ADF test was below the threshold, indicating that the series is stationary.
- **Interpretation**: A stationary series is suitable for ARIMA and ARIMAX models.

### ACF and PACF Analysis

- **Autocorrelation Function (ACF)** and **Partial Autocorrelation Function (PACF)** plots were used to determine the p (autoregressive) and q (moving average) orders.
- **Result**: Low values for p and q were selected based on the plots.

### Daily New User Forecasting with ARIMA

- **Model Training**: ARIMA model was trained on daily new user data.
- **Parameter Selection**: The optimal (p, d, q) parameters were determined as (1, 1, 1).
- **Forecasting**: Daily new users were forecasted for the next 30 days.

### DAU Forecasting with ARIMAX

- **Exogenous Variable**: Daily new user counts were used as an auxiliary variable in the ARIMAX model.
- **Model Training**: ARIMAX model was trained on DAU data.
- **Parameter Selection**: The optimal (p, d, q) parameters were determined as (2, 0, 0).
- **Forecasting**: DAU was forecasted for the next 30 days.

## Results and Insights

- **Model Performance**: Both ARIMA and ARIMAX models demonstrated strong performance with low error rates on test data.
- **Forecasts**: The predictions provide actionable insights into future user engagement and growth trends.
- **Business Value**: These forecasts can help shape marketing and product development strategies.

## Contact

- **Project Owner**: Çiya Baran Öner
- **Email**: [ciya.baran.oner@gmail.com](mailto:ciya.baran.oner@gmail.com)
- **LinkedIn**: [linkedin.com/in/ciyabaranoner](https://linkedin.com/in/ciyabaranoner)
