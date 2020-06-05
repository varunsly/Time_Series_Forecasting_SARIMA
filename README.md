# Time_Series_Forecasting_SARIMA
Using SARIMA model for time seies forecasting

# About

**SARIMA** (Seasonal Autoregressive Integrated Moving Average) is an extension of the ARIMA.
For this model, I have used SARMIAX to have more flexibility.

* **Agumented Dickey Fuller Test** is used to check the whether the dataset is stationary or not.

* Different methods are implemneted to make the non-stationary data stationary:

   * Log Transform
   
   * Rolling mean
   
   * First Difference, Seasonal Difference
   
* Then, ACF and PACF graphs are plot to estimate the SARIMAX parameters. After, the estimation the parameters are selected to train the model.

**GridSearchCV** is used to serach the more optimized parameters. The **AIC**(Akaike information criterion) is used as the benchmark to select the best parameters for the model

**Walk_Forward_Validation** method is also used to increase the efficiencey of the model

***The model(GridSearchCV or Walk_Forward_Validation) with the least **Mean Absolute Error and Mean Absolute Percent Error** is selected for making the forecasting***
### Dataset
 
***For training and testing this model, the data has been taken from the[Federal Reserve Economic Data](https://fred.stlouisfed.org/)***

## Note
 * The predictions made through the Walk_Forward_Validation are still in log form.
 * They needed to transformed to show better graphical relation
 
 **The Code Will be updated Soon**
