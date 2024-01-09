# Various Models and Accuracy Evaluation, using Performance Metrics

## Overview
This project attempts to model the time series of *unemployment rate among college graduates*, who are aged between 20-24 and have bachelor's degree and higher. The time series spans across the past 23 year, from 2000 to 2023, and the observation frequency is monthly. The primary focus of this project is to apply various modeling methods and finding the best performing forecasting model that could potentially perform well on the unknown future data. For the project purposes, 7 forecasting models were selected, including:

1. STL + ARMA Model
2. ARIMA Model
3. ETS Model
4. Holt-Winters Model
5. Neural Network Autoregressive Model
6. Prophet Model
7. Combined Model

To assess the performance of each model, the test-train split procedure was used, and the ratio of the split was; train: 80% and test: 20%. The performance of each model was numerically measured by performance metrics, specifically ME, RMSE, and MAE, and the preferred model was also selected based on the result.




## Data
The dataset used for this project are downloaded from the FRED Economic data website 
1. https://fred.stlouisfed.org/series/CGBD2024

The observation frequency of the data is monthly and was preprocessed for analysis.

## Methodology


#### STL + ARIMA Model
- This model combines Seasonal-Trend decomposition using Loess (STL) and Autoregressive Integrated Moving Average (ARIMA) methods. STL decomposes the time series into seasonal, trend, and remainder components, and ARIMA models the residuals to capture any remaining patterns.
  
#### ARIMA Model
- Autoregressive Integrated Moving Average (ARIMA) model uses differencing to make time series stationary and fits AR (Autoregressive) and MA (Moving Average) parameters.
  
#### ETS Model
- Error-Trend-Seasonal (ETS) models capture the error, trend, and seasonal components of a time series. ETS model handles various patterns, including exponential smoothing, trend decay, and seasonality.
  
#### Holt-Winters Model
- The Holt-Winters model considers the error, trend, and seasonality components of a time series.
  
#### Neural Network Model
- Nueral Network Autoregressive (NNAR) models are based on simple mathematical models of the human brain. This model can learn from the historical data and make predictions based on the patterns identified

#### Prophet Model
- Prophet is a forecasting model developed by Facebook that handles time series data with daily observations that display patterns such as seasonality and holidays. In other words, this model is designed for high frequency data.
  
#### Combined Model
- Combined model leverage individual strenghts. In this project, a simple averaging method is used.
  
#### ARCH/GARCH Model
- Autoregressive Conditional Heteroskedasticity (ARCH) and Generalized Autoregressive Conditional Heteroskedasticity (GARCH) models are used for modeling volatility.



