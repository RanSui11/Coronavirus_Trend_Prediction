# Coronavirus Trend Prediction

Access the app here: [https://hxiong6.shinyapps.io/dsproject/](https://hxiong6.shinyapps.io/dsproject/)   
Access the presentation here: [https://drive.google.com/file/d/1L4v0GXLsv7oj_Gmnb7GMZ5sd_Ef5fBt1/view](https://drive.google.com/file/d/1L4v0GXLsv7oj_Gmnb7GMZ5sd_Ef5fBt1/view)  



## Library requirements

flexdashboard; plotly; shiny;e1071; ggplot2; tidyverse; rvest;highcharter

## Shiny App description

This app displays the prediction of confirmed Covid-19 cases for the week ahead. 
#### Sidebar
1. The sidebar displays when the data in the app was last updated.
2. Select state of which you are interested to see the trend of confirmed cases.
3. A United States map shows the total confirmed cases of 50 states. Values are in k scale. 
#### United States
1. In prediction part, the interactive plot will display the cumulative cases of Covid-19 of the state you choose since Jan,22,2020 and two predicted trends for the week ahead by SVM model and GLM model.
2. In US data, the table shows the number of confirmed cases for last 7 days.
####  World Data
1. The table summarize the confirmed coronavirus data around the globe.
#### About
1. Overview of the project, disclaimer of the app, and references used through the project.

## Project description

#### Data processing
1. Filter the data of the state user wants and combine them.
2. Model learns from the date in which the number of confirmed cases is greater than 0.
#### Algorithms
1. SVM: Use polynomial kernel and tune parameters of c and gamma by using trial and error. Implement the optimal SVR model to predict the confirmed case for the week ahead.
2. GLM: Use quasipoisson model. Assume that the response variable Y (cumulative confirmed cases) follows a poisson distribution, and the logrithm of its expected value can be modeled by a linear combination of parameters.  

## Access to the data
1. Data for prediction model [https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_US.csv](https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_US.csv)  
2. Data for USA [https://www.worldometers.info/coronavirus/country/us/](https://www.worldometers.info/coronavirus/country/us/)  
3. Data for globe. [https://www.worldometers.info/coronavirus/](https://www.worldometers.info/coronavirus/)

## Member contribution
Ran Sui: SVM model; United states section;Flexdashboard making      
Hao Xiong: GLM model;World section, resource and disclaimer section; Flexdashboard making
