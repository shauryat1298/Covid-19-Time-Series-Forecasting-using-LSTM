
# Time Series Analysis for Covid-19 using LSTM

From March 2020, the world has seen a major shift in dynamics. We saw the upsurge of Covid-19, which caused a global crisis. This project focuses on the analysis of Covid-19 dataset.

### The project is divided into 2 parts:
1. Exploratory Data Analysis
2. Time series forecasting using long short-term memory (LSTM)

![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/lstm.png?raw=true)
## Dataset used:
I have used 2 different datasets for the divided tasks:

1. NYC Coronavirus Disease data (https://github.com/nychealth/coronavirus-data)
2. Covid-19 Global Forecasting data (https://www.kaggle.com/competitions/covid19-global-forecasting-week-4/data)

## Exploratory Data Analysis

Fist task was to create a world map of Covid-19 cases distribution for "Confirmed Cases" and "Fatalities"

![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/Confirmed%20Cases%20in%20Different%20Countries%20(Jan-May%202020).png?raw=true)
![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/Fatalities%20in%20Different%20Countries%20(Jan-May%202020).png?raw=true)

### Continental distribution using Lineplots:

Green - Confirmed Cases  
Red - Fatalities

![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/continentwise_analysis_lineplot.png?raw=true)

* Our analysis shows 'Europe' as the continent with the maximum confirmed cases and fatalities.  
* Asia shows a spike in confirmed cases around February 15, 2020, due to sudde spike in cases in China.

### Country wise comparison for Confirmed Cases and Fatalities
Green - Confirmed Cases  
Red - Fatalities

![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/countrywise_analysis_lineplot.png?raw=true)

* Italy has the maximum Confirmed Cases and Fatalities.  
* Germany had an equivalent number of confirmed cases as Italy, but the fatalities were in much control.
* Turkey had a big amount of confirmed cases, but they managed the fatalities fairly well. Same goes for Russia.

### Barplot on the Fatalities in the States of USA

![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/Fatalities%20by%20States%20(USA)%20(Jan-May%202020).png?raw=true)

* New York had the maximum number of fatalities of ~60K
* Massachusetts, Michigan, Pennsylvania, Illionis, California had measurable fatalities ~10K

### Covid-19 Confirmed Cases by States
![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/COVID-19%20Confirmed%20Cases%20by%20States.png?raw=true)

## EDA based on Race, Age, Sex, Poverty

### AGE Factor: New York (Confirmed Cases v/s Fatilities)
![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/age.png?raw=true)
* Confirmed cases shows close to a normal distribution which shows that every age group was equally affected.
* People in the higher age groups were the most affected by deaths

### RACE Factor: New York (Confirmed Cases v/s Fatilities)
![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/race.png?raw=true)
* There's no distinction in confirmed cases and fatalities due to different races

### GENDER Factor: New York (Confirmed Cases v/s Fatilities)
![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/gender.png?raw=true)
* Female population had more number of confirmed cases as compared to Male population
* On the contrary, fatalities were more in the Male population as compared to Females

### POVERTY Factor: New York (Confirmed Cases v/s Fatilities)
![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/poverty_level.png?raw=true)
* There's no distinction in confirmed cases and fatalities due to different poverty
* We can conclude that no proper cure was developed, since money was not a distinguishing factor
## Time Series Analysis using LSTM RNN

We plotted a line plot for the predicted values v/s actual values for Confirmed cases and Fatalities

### Predicted v/s Actual values (Confirmed Cases)
![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/Predicted%20Values%20VS%20Actual%20Values%20-%20Confirmed%20cases.png?raw=true)

### Predicted v/s Actual values (Fatalities)
![](https://github.com/shauryat1298/Covid-19-Time-Series-Forecasting-using-LSTM/blob/main/figures/Predicted%20Values%20VS%20Actual%20Values%20-%20Fatalities.png?raw=true)

As we can see, the forecasted values were close enough to the actual values, displaying the power of using LSTM RNNs for prediction models