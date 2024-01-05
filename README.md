# Project Name
> Bike Sharing Assignment


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
BoomBikes, a US bike-sharing provider, aims to recover from pandemic-induced revenue declines with a strategic plan. The focus is on post-lockdown demand for shared bikes in the American market, identifying key variables and their impact. Objectives include determining predictive variables and assessing their effectiveness in describing bike demands. 

The project's goal is to model shared bike demand using available independent variables, enabling management to adapt strategies, meet customer expectations, and understand new market dynamics. The dataset for analysis is available [here](day.csv).

## Technologies Used
- python 3.11.4
- jupyter notebook
- pandas 1.5.3
- numpy 1.24.3
- matplotlib 3.7.1
- seaborn 0.12.2
- statsmodels 0.14.0
- sklearn 1.3.0

## Conclusions
- The linear regression model developed to predict the bike demand has a predictive power(adjusted R-square) of 83.20%
- The various independent variables that impact the bike demnand are temp, windspeed, summer, spring, yr, winter, July, mist, September, Monday, light snow.
- The linear model is as follows:

     __cnt = 0.2036 + (0.4923)temp - (0.1498)windspeed + (0.0467)summer - (0.0680)spring + (0.2338)yr + (0.0831)winter - (0.0486)July
    -(0.0816)mist + (0.0721)September - (0.0451)Monday - (0.2856)light snow__
- From the above model it can cleary be seen that the top 3 contributer are:
    - **Year(yr)** : Since the coefficient is positive, it means from 2018 to 2019 the demand for bikes has increased.
    - **Light Snow (light snow)** : Weather situation - "Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds" is also a significant contributor. The negative coefficient indicates that during light snow conditions, the demand for shared bikes decreases. This is understood, as snowy weather can lead to less number of bikes used.
    - **Temperature (temp)** : The positive coefficient implies that as the temperature increases, the demand for shared bikes also increases. Warm days can see increased demand for bikes. This is in sync with light snow weather situations, as temp generally decreases in such situations leading to drop in bikes demand. 

## Contact
Created by [prachigithub](https://github.com/prachigithub/) - feel free to contact me!