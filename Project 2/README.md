# VAR model (Granger Causality Analysis)

## Overview
This project explores two respective time series datasets of monthly export trades for Indonesia and Korea, from 1990 to 2023. Using the VAR model, Granger Causality analysis, and IRF (Impulse Response Function), it analyzes if there is any statistically significant causal relationship between the time series, such that the behavior of one series can help explain the other's future values. Lastly, it attempts to forecast the unknown future values using the VAR model built within the project.



## Data
Both of the datasets used for this project are downloaded from the FRED Economic data website 
1. https://fred.stlouisfed.org/series/XTEXVA01IDM667S
2. https://fred.stlouisfed.org/series/XTEXVA01KRM667S
   
The observation frequency of the data is monthly and was preprocessed for analysis.

## Methods


#### VAR Model Construction
The core modeling technique employed in this project is the Vector Autoregression (VAR) model. VAR models are well-suited for capturing the dynamic interdependencies between multiple time series. The model was fitted on the preprocessed data.

#### Granger Causality Analysis
Granger Causality analysis was conducted to verify whether past values of one time series provide statistically significant information for predicting the future values of the other. 

#### Impulse Response Function (IRF)
The Impulse Response Function was utilized to examine the reaction of each variable in the system to a one-time shock in another variable. This analysis provides insights into the dynamic responses and interactions between the two economic indicators over time.

