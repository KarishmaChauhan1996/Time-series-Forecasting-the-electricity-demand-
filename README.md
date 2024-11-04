**Time Series Analysis and Forecasting**

This project involves analyzing and forecasting future demand for a time series dataset of Electricity demand.
We utilize various statistical and machine learning techniques to capture trends, seasonality, and other patterns in the data, with the goal of making accurate future predictions.

**Project Overview**

The objective of this project is to perform comprehensive time series analysis and forecasting on a given dataset. We explore the data, preprocess it, and apply various models to forecast future values. The project demonstrates the use of common forecasting methods and assesses their performance using error metrics to identify the best model for the dataset.

**Table of Contents**

Project Overview

Data

Usage

Methodology

Models Used

Evaluation Metrics

Results

Conclusion

License

**Data**

The dataset used in this project includes time-based data with one time series attributes. Columns in the dataset include:

Date/Time: The timestamp or date at which each observation was recorded.

Target Variable: The main variable to be forecasted (Electricity_Demand_in_TW).

**Usage**

pandas

numpy

matplotlib

datetime

seaborn

re

statsmodels

**Methodology**

This project involves the following steps:

1. Data Cleaning and Preprocessing: Handle missing values if any, handle Datetime column for data type.

2.  Exploratory Data Analysis: Visualize the data to understand trends, seasonality, and any cyclic behavior.
![trend](https://github.com/user-attachments/assets/1fee00b2-25c8-4246-8cef-49e389149753)
![yearly_consumption_trend](https://github.com/user-attachments/assets/32ec00fa-d078-4fe8-a023-31c86c7c8c3f)
![seasonal_trend](https://github.com/user-attachments/assets/6e4ced30-6ed9-4c1f-a910-669048f8c2a6)
![decompose](https://github.com/user-attachments/assets/7d2a410e-7d32-4074-989a-5f424031a33a)
![decompose_additive](https://github.com/user-attachments/assets/7934b28e-3f99-422c-84df-68482a318a4e)

3.Quantify relationship of data with past values:

       Autocorrelation, Partial Autocorrelation.

  ![autocorrelation_ts](https://github.com/user-attachments/assets/d28f1373-f723-45fd-9471-440a8637e6bc)

  ![partialAutocorrelation_ts](https://github.com/user-attachments/assets/4e8db8ea-66e1-42f0-9789-a59992789e89)

     
4. Dickey Fuller test: To check seasonality in the data.
   
5. Make series stationary

        Logarithmic transformation
   
        Moving Average

 Moving average trend
 
 window=24

![rolling_stat-MovingAverage](https://github.com/user-attachments/assets/a05ced2f-3b36-4abd-a3b7-fb9b4020c860)

window=12

![rollingStat-MovingAverage-Window12](https://github.com/user-attachments/assets/2c4dd6f6-cd2b-4850-adba-dd1aab21651a)

window=9

![rollingStat-MovingAverage-Window9](https://github.com/user-attachments/assets/a7609db7-792b-4445-8bd3-860ad5848424)

window=6

![rollingStat-MovingAverage-Window6](https://github.com/user-attachments/assets/c06ee90b-99a9-4718-8df2-5a52ab029496)

   
6. Model Selection and Training:

7. Fit time series models to the data and select best fit model.

8. Model validation: Generate forecasts for next 5 months and calculate forecasting error.

9. Prediction: Predicting demand of electricity for next 12/24 months.
10. Model Evaluation: Compare model performances based on error metrics.

**Models used**

        ETS(Exponential Smoothing State Space Model)
        
        SARIMAX (Seasonal Autoregressive Integrated Moving Average with Exogenous Regressors Model)

![ETS_summary](https://github.com/user-attachments/assets/9a622237-82a3-406a-8c95-33a7a30cbe07)

![SARIMAX](https://github.com/user-attachments/assets/51c3d00d-e437-425b-893f-fd911c0c1fb7)
        
**Evaluation Metrics**

We use several error metrics to assess model performance:

RMSE (Root Mean Square Error)

MAPE (Mean Absolute Percentage Error)

RMSPE (Root Mean Square Percentage Error)

**Results**



**Conclusion**

This project provides a comprehensive approach to time series analysis and forecasting. Through this analysis, we identified the best model for our dataset, allowing us to generate reliable forecasts. Further steps could include tuning model parameters, experimenting with more complex models, and applying this methodology to different datasets


