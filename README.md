# Time series forecasting project

This is a project I did on time series forecasting.
I chose the Individual Household Electric Power Consumption Data Set
from the UCI repository as my data set. My goal was to predict the daily 
active power usage of a household.

## Results

I implemented and tested 3 time series forecasting methods: A classical ARIMA
model, coupled with a decomposition of the time series, the prophet library from Facebook
and a custom neural-network based model based on a 2-layer bidirectional LSTM.

To compare the three methods, I also measured the baseline of a persistence model; that is,
to just forecast the data by repeating the last value.
The results were (on a test set):

* Baseline: RMSE of 411.92
* ARIMA: RMSE of 385.74
* Prophet: RMSE of 376.52
* LSTM: RMSE of 283.27

Plots and results are shown in the Jupyter notebook, which also contains the code for the project.
