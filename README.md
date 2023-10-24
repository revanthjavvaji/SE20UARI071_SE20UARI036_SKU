# SE20UARI071_SE20UARI036_SKU_Assign
# Time Series Forecasting with ARIMA and Exponential Smoothing (ETS)

This repository contains code for time series forecasting using two different models: ARIMA (AutoRegressive Integrated Moving Average) and Exponential Smoothing (ETS). The code demonstrates how to train, evaluate, and make sales forecasts for a specific store and department combination.

## Dataset
The code uses a dataset named `train.csv`, which contains the following columns:
- Store: Store number
- Dept: Department number
- Date: Date of sales data
- Weekly_Sales: Weekly sales amount
- IsHoliday: Indicator for special holiday weeks

`train.csv` is taken from Kaggle.The code preprocesses the data by handling missing values and encoding the `IsHoliday` column.

Source:  [Dataset](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data?select=train.csv.zip)

## ARIMA Model
The ARIMA model is used for time series forecasting. The code provides functions to train and evaluate the ARIMA model. It calculates the Mean Absolute Error (MAE) and provides sales forecasts for the next 12 weeks.

### Training the ARIMA Model
To train the ARIMA model for a specific store and department, use the `train_arima_model` function.

### Evaluating the ARIMA Model
The `evaluate_arima_model` function is used to evaluate the ARIMA model's performance on test data. It calculates MAE and provides sales forecasts.

## Exponential Smoothing (ETS) Model
The Exponential Smoothing (ETS) model is another time series forecasting approach. Similar to the ARIMA model, the code includes functions for training and evaluating the ETS model.

### Training the ETS Model
To train the ETS model for a specific store and department, use the `train_ets_model` function.

### Evaluating the ETS Model
The `evaluate_ets_model` function is used to evaluate the ETS model's performance on test data. It calculates MAE and provides sales forecasts.

## Usage
To use this code for time series forecasting, follow these steps:
1. Ensure you have the `train.csv` dataset or replace it with your data.
2. Run the code in your Python environment.
3. Adjust the store and department parameters for training and evaluation.
4. Review the MAE and sales forecasts for each model.

Feel free to customize the code for your specific forecasting tasks and datasets.

## Dependencies
This code uses the following Python libraries:
- pandas
- statsmodels

You can install these dependencies using `pip` if you haven't already.

## Summary of Results

### ARIMA Model
- **Mean Absolute Error (MAE):** 3437.25 (approximately)
- **Sales Forecast for the Next 12 Weeks:**
  - Week 1: 21313.97
  - Week 2: 21457.75
  - Week 3: 18754.76
  - Week 4: 19434.22
  - Week 5: 19750.00
  - Week 6: 19930.99
  - Week 7: 20191.15
  - Week 8: 19622.24
  - Week 9: 19637.39
  - Week 10: 19864.92
  - Week 11: 19825.75
  - Week 12: 19860.95

### ETS Model
- **Mean Absolute Error (MAE):** 2402.12 (approximately)
- **Sales Forecast for the Next 12 Weeks:**
  - Week 1: 16602.63
  - Week 2: 12322.99
  - Week 3: 14337.87
  - Week 4: 17933.35
  - Week 5: 14385.70
  - Week 6: 15937.91
  - Week 7: 13183.54
  - Week 8: 18858.51
  - Week 9: 40885.94
  - Week 10: 22606.91
  - Week 11: 26347.84
  - Week 12: 18634.32

## Issues Faced
The main issues faced were data preprocessing complexities, including handling missing values, and selecting optimal hyperparameters for the ARIMA and ETS models, which greatly affected forecasting accuracy.

## Steps Taken
1. The code imports necessary libraries, loads the dataset, and performs data preprocessing (handling missing values and converting data types).
2. Two forecasting models are trained and evaluated: ARIMA and ETS.
3. MAE is calculated to assess the accuracy of the forecasts.
4. Sales forecasts are provided for the next 12 weeks for each model.





---

This README provides an overview of the time series forecasting code using ARIMA and ETS models. 
