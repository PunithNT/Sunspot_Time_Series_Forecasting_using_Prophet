# Sunspot_Time_Series_Forecasting_using_Prophet
This repository implements a time series forecasting model using Facebook's Prophet library to predict sunspot numbers. It forecasts future sunspot values based on historical data from daily, monthly, and yearly datasets, leveraging FBProphet to model non-linear trends with various seasonality (yearly, weekly, daily).

# Project Overview
The main goal of this project is to forecast future sunspot numbers and evaluate the performance of the model using different time periods and granularities. The dataset includes historical data on sunspot numbers at different time scales (daily, monthly, and yearly) and provides insights into future solar activity based on past patterns.

# The project includes:

**Data Loading & Preprocessing**: Read and preprocess sunspot datasets (Daily, Monthly, Yearly).
**Prophet Model**: Train and predict using Prophet for each dataset with time-dependent predictions (100/200/365 days for daily, 1/6/9 months for monthly, and 1/10/20 years for yearly).
**Model Tuning**: Apply hyperparameter tuning for forecasting growth, seasonality, and trend changepoints.
**Evaluation Metrics**: Evaluate model performance using MAE (Mean Absolute Error), MAPE (Mean Absolute Percentage Error), and R² (coefficient of determination).
**Visualization**: Visualize predictions and historical data to track forecast accuracy.

# Datasets
**Daily Sunspot Data**: SN_d_tot_V2.0.csv
**Monthly Mean Sunspot Data**: SN_m_tot_V2.0.csv
**Yearly Mean Sunspot Data**: SN_y_tot_V2.0.csv
These datasets contain sunspot numbers collected over time, with daily, monthly, and yearly observations. The datasets are used to train and test the forecasting models.

# Usage
Daily Sunspot Forecasting: Run daily_forecasting.ipynb to forecast sunspots for the next 100, 200, and 365 days.
Monthly Sunspot Forecasting: Run monthly_forecasting.ipynb to forecast sunspots for the next 1, 6, and 9 months.
Yearly Sunspot Forecasting: Run yearly_forecasting.ipynb to forecast sunspots for the next 1, 10, and 20 years.

# Model Evaluation
The performance of the model is evaluated using the following metrics:

**Mean Absolute Error (MAE)**: Measures the average of the absolute errors between predictions and actual values.
**Mean Absolute Percentage Error (MAPE)**: Measures the percentage of the error relative to the actual values.
**R² (Coefficient of Determination)**: Measures the proportion of variance in the dependent variable that is predictable from the independent variables.

# Hyperparameter Tuning
Hyperparameters are tuned to optimize the forecast:

**Growth**: Linear or Logistic growth.
**Seasonality**: Custom seasonality based on solar cycles.
**Changepoint Prior Scale**: Controls the flexibility of the trend.
**Fourier Order**: Controls the complexity of the seasonal effects.

# Contribution
Feel free to fork this repository and contribute by creating pull requests. If you find bugs or issues, open an issue so we can address them.





