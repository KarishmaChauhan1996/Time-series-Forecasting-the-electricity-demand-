Time Series Analysis and Forecasting

This project involves analyzing and forecasting future demand for a time series dataset of Electricity demand.
We utilize various statistical and machine learning techniques to capture trends, seasonality, and other patterns in the data, with the goal of making accurate future predictions.

Project Overview

The objective of this project is to perform comprehensive time series analysis and forecasting on a given dataset. We explore the data, preprocess it, and apply various models to forecast future values. The project demonstrates the use of common forecasting methods and assesses their performance using error metrics to identify the best model for the dataset.

Table of Contents
Project Overview
Data
Usage
Methodology
Models Used
Evaluation Metrics
Results
Conclusion
License

Data
The dataset used in this project includes time-based data with one time series attributes. Columns in the dataset include:

Date/Time: The timestamp or date at which each observation was recorded.
Target Variable: The main variable to be forecasted (Electricity_Demand_in_TW).

Usage
pandas
numpy
matplotlib
datetime
seaborn
re
statsmodels

**Methodology**

This project involves the following steps:

Data Cleaning and Preprocessing: Handle missing values if any, handle Datetime column for data type.
Exploratory Data Analysis: Visualize the data to understand trends, seasonality, and any cyclic behavior.
![trend](https://github.com/user-attachments/assets/1fee00b2-25c8-4246-8cef-49e389149753)

Quantify relationship of data with past values: Autocorrelation, Partial Autocorrelation.
Dickey Fuller test: To check seasonality in the data.
Make series stationary
        Logarithmic transformation
        Moving Average
Model Selection and Training: Fit time series models to the data and select best fit model.
Model validation: Generate forecasts for next 5 months and calculate forecasting error.
Prediction: Predicting demand of electricity for next 12/24 months.
Model Evaluation: Compare model performances based on error metrics.

Models used

        ETS(Exponential Smoothing State Space Model)
        SARIMAX (Seasonal Autoregressive Integrated Moving Average with Exogenous Regressors Model)
        
Evaluation Metrics

We use several error metrics to assess model performance:

RMSE (Root Mean Square Error)
MAPE (Mean Absolute Percentage Error)
RMSPE (Root Mean Square Percentage Error)

Results



Conclusion

This project provides a comprehensive approach to time series analysis and forecasting. Through this analysis, we identified the best model for our dataset, allowing us to generate reliable forecasts. Further steps could include tuning model parameters, experimenting with more complex models, and applying this methodology to different datasets


