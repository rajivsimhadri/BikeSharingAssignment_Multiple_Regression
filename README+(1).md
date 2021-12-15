# Bike-Sharing System
> To build a multiple linear regression model for the prediction of demand for shared bikes.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

- A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.
                                                    They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
    1) Which variables are significant in predicting the demand for shared bikes.
    2) How well those variables describe the bike demands
 
- Business Goal:
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market. 

- Bike Sharing dataset(# day.csv).

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- library - pandas
- library - numpy
- from pandas_profiling import ProfileReport
- from statsmodels.formula.api import ols
- from sklearn.preprocessing import MinMaxScaler
- from sklearn.feature_selection import RFE
- from sklearn.linear_model import LinearRegression
- from statsmodels.stats.outliers_influence import variance_inflation_factor
- from sklearn.metrics import r2_score

## Conclusions
1) We can clearly see that only 15 features were selected over 30 features after doing some feature engineering.
2) See the above cell for list of final features
3) The Final Model has an Adjusted R2 of 0.842 which performed on the test set with an R2 score of 0.847
4) The r2_score for the model on test set , we got a value of 0.81

### Feature Wise importance:
The following variables have negative impact on the final model, as we can see the lm coefficient params
Rainy, windspeed , hum , mist , nov ans Dec(maybe due to holiday seasons)
20% negative impact is due to the windspeed
15% negative impact is due to the hum
In the year 2019, we could see around 23% increase in the count of the riders.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact
Created by [@rajivsimhadri] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
