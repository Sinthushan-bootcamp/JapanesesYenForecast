# A Yen for the Future

In this project we are attempting to predict YEN/CAD futures using ARMA, ARIMA, GARCH and Regression analysis.

Raw data used for the analysis can be found here: [CAD/JPY Data CSV File](cad_jpy.csv)

The ARMA, ARIMA and GARCH models can be found here:[Time-Series Starter Notebook](time_series_analysis.ipynb)

The ARMA and ARIMA did not have much predictive value as the P-value was significanlty more than 0.05 for the two lags that we applied, regardless they pboth seemed to predict the Japanese Yen going down. THe GARCH model faired better with a P-value much lower then 0.05 for lag 1. THe GARCH model predicted an increase in volatitlity.

We conclude from the analysis that buying yen would be a poor decision as it is predicted to go down as well as being highly volatile.


The Regression analysis can be found here [Linear Regression Starter Notebook](regression_analysis.ipynb)

For the regression analysis we split the data into training and test samples using data from before 218 as our training data and all data points after 2018 as out test data.Based on the out of sample and in sample RMSE. We see that the model performed better with out of sample data than with in sample data