# RainFall-Time-Series

# AI PROJECT ON RAINFALL TIME SERIES :-
# BUSINESS CASE: Time series forecasting model to predict next month's rainfall based on historical data.
## PYTHON IMPLIMENTATION :-
* Load Data
* Check The Basics of data
##  VISUALISE TREND OF RAINFALL :-  
![image](https://github.com/user-attachments/assets/9e307bee-58ed-4f2e-a838-4e0d6c2402f2)
### Observation :-
* The Data is shows the strong Seasonality.

## Visualise the different components like seasonal nature, trend for that we are use stats model :-
### Seasonal Decomposition :-
* A time series data is composed of
    * Trend: Trend is the overall direction of the data.
    *  Seasonlity: Seasonality is a periodic component which repeats itself            within a particulat time period.
    * Residuals: the residual is what’s left over when the trend and                 seasonality have been removed. Residuals are random fluctuations.
![image](https://github.com/user-attachments/assets/01c25dd0-bf2b-448e-9eeb-4e44f6335d69)
![image](https://github.com/user-attachments/assets/23f0a6e7-b675-4e25-9ba2-38fc925719dd)
![image](https://github.com/user-attachments/assets/2c004481-f458-4e5f-abd3-c468010331b9)

 
## SPLIT DATA INTO TRAIN & TEST :-
* Train test split in timeseries is different as copared to Machine learning Algforithms. We do random split there where the time component does'nt matters. But in time series we have information dependent on time therefore the spliting is continous without any shuffling of data.

   * Taking last 12 month data for testing and remaining data for training
   * Using 37 years data for training (1982-01-01 to 2019-06-01)
   * Using 1 year data for Testing (2019-06-01 to 2020-06-01)
 
## MODEL CREATION :-
* In this project we are use SARIMAX to predict the mean of maximum_rainfall_in_a_day, no_of_rainy_days And total_rainfall .

* Creating a batches of 12 months with the help of arima-order and seasonal-order by using the auto_arima method from the pmdarima-library .

## COMPILE & TRAIN MODEL :-

## PREDICTION :-
* Forecast for 2021 :-
![image](https://github.com/user-attachments/assets/469c87a8-cb4c-441e-9fe9-a8f3e4b12e47)
* Take last 12 months values to make a prediction of first value of test set and make prediction .

## CHALLENGES :-
* Problem Faced To Understand the Business case
* First time worked with time series data
* Problem faced to make prediction

## LEARNING FROM THIS PROJECT :-
* Learn time series prediction using SARIMAX.
* Learn how to do monthly prediction.

## MODEL SAVEING :-
* Save the SARIMAX models to separate files using pickle.
