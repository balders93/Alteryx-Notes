# Alteryx Notes

## Time Series
– Investigate data first, would want to address any missing values before diving in with some form of imputation
– Two possible models
– ARIMA: autoregressive integrated moving average (more common)
– ETS: Exponential Smoothing
– Can use TS Compare to compare both models on test data.
– Configuration of models: Give it a name, select your target field to forecast, select target frequency (daily, weekly, monthly etc)
– Other Options: How many periods ahead you want to forecast.
– TS Compare: union both model outputs and put them into the left input, put your test data into the right input.
– The results give you various different measures of ‘error’ for each one lower is better.
– Take your better model then put the O output through “TS Forecast” Tool.
