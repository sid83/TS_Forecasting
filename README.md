# TS_Forecasting
Time series forecasting was done using Seasonal ARIMA model. FOllowing steps were followed.

* Data imported and cleaned. Unnecessary columns were removed.
* Time series was decomposed into trend, seasonal and remainder components. This was done to figure out the significant components of this ts. TS was found to contain linear trend and a seasonality of 12 months.
* Grid search to identify the most optimal order of the SARIMA model. Minimum AIC was chosen as a criteria for selecting the model. Other criteria may be to choose the model based on minimum MSE (will be tried later).
* Once optimum model is identified, "one step ahead" forecasts were carried out and mean square error (mse) calculated. 
* Then dynamic forecasts were calculated and corresponding mse calculated.
* Low value of both MSEs verified and validated the selected model.
* Finally forecasts for future 500 steps were carried out and plotted along with the 95% confidence interval.
* Python library, Statsmodel was used for SARIMA modelling. 