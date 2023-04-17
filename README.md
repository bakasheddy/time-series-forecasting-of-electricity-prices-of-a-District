# <center>Time Series Forecasting of Electricity Prices of a District</center>
### <center>by</center>
## <center>Shedrack David</center>


## Project Overview

This data set was provided by Hamoye where i did my internship as a test of our time-series analysis skill.
the data contains 92016 entries and 5 columns which consists of FullDate, Tmax,	SysLoad, GasPrice and ElecPrice as column names.
the dataset captures the power consumption of a building for a period of 11 years (2010 - 2021)

Apart from the FullDate column, every other column is of thr float data type, the FullDate column was converted from object(string) to datetime format before exploration
The goal of this project was to forecast the electric price for a district using time-series data. The data was checked for stationarity using the Augmented Dicky Fuller test, and it was found to be fairly stationary. However, to make the data more stationary, differencing was applied. The fbprophet library was used to build a forecasting model, which was then evaluated using various metrics.

## Aim

In this project, i will explore and build time series forecasting model for measurements of electric power consumption in one household with a one-minute sampling rate over a period of almost 4 years.

## Objective

To achieve what i aim for, i used Facebook's prophet to build my model and train it on 9 years of the dataset (2010 - 2019), the testing data will be done on the two remaining years

## Evaluation Metrics:
The model's performance was evaluated using three metrics: Mean Absolute Error (MAE), Mean Absolute Percentage Error (MAPE), and Root Mean Squared Error (RMSE).

## Evaluation Results:
The evaluations of the FBProphet model are as follows:

MAE: 70.817

MAPE: 223.174%

RMSE: 91.507
## Analysis:
Based on the evaluation metrics, the FBProphet model performed moderately well in forecasting the Electric Price of the building. The MAE value of 70.817 indicates that on average, the model's predictions were off by around 71 units. The MAPE value of 223.174% suggests that the model's predictions were, on average, 223% off from the actual sales figures. Finally, the RMSE value of 91.507 indicates that there was a root mean squared error of 92 units in the model's predictions.

## Conclusion:
While the fbprophet model provided a good starting point for the project, the evaluation results show that it may not be accurate enough for reliable predictions.  However, there is still room for improvement. The model's evaluations suggest that it may be overestimating or underestimating the Electric prices. In order to improve the model's accuracy, further exploration and experimentation with different algorithms, models, and parameters is recommended.
