# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal was to find a correlation between bike availability and being near schools and/or bars

## Process
### City Bikes
1. Review the website and API documentation
2. Develop the code to create the request for the city selected
3. Export data into CSV
### Foursquare
1. Review the documentation and figure out which URL I needed to pull
2. Develop a request that pulled results for one location to see structure of return
3. Figured out the map for accessing the information I needed
4. Wrote code that iterated through the station data and pulled POIs for each station
5. Created a dataframe with parsed data
6. Checked for duplicates
### Yelp
1. Review the documentation and figure out which URL I needed to pull
2. Develop a request that pulled results for one location to see structure of return
3. Figured out the map for accessing the information I needed
4. Wrote code that iterated through the station data and pulled POIs for each station
5. Created a dataframe with parsed data
### EDA
1. Outlined basic data to check for outliers and get a sense of the dataset individually and then when merged as well. 
2. Created graphs and images to visualize the data.
### Model Creation
1. I opted to create a model based on empty bikes and ratings from foursquare and yelp and also if the location was a school or a bar. 

## Results
                            OLS Regression Results                            
==============================================================================
Dep. Variable:             free_bikes   R-squared:                       0.488
Model:                            OLS   Adj. R-squared:                  0.473
Method:                 Least Squares   F-statistic:                     33.36
Date:                Mon, 21 Oct 2024   Prob (F-statistic):           1.57e-19
Time:                        18:09:21   Log-Likelihood:                -384.73
No. Observations:                 145   AIC:                             779.5
Df Residuals:                     140   BIC:                             794.3
Df Model:                           4                                         
Covariance Type:            nonrobust                                         
=================================================================================
                    coef    std err          t      P>|t|      [0.025      0.975]
---------------------------------------------------------------------------------
const            -1.6389      3.406     -0.481      0.631      -8.373       5.095
rating_foursq     0.4154      0.316      1.315      0.191      -0.209       1.040
rating_yelp      -0.3484      0.533     -0.653      0.515      -1.403       0.706
distance_yelp    -0.0047      0.003     -1.811      0.072      -0.010       0.000
slots.1           0.4715      0.044     10.758      0.000       0.385       0.558
==============================================================================
Omnibus:                        5.899   Durbin-Watson:                   0.470
Prob(Omnibus):                  0.052   Jarque-Bera (JB):                5.697
Skew:                           0.483   Prob(JB):                       0.0579
Kurtosis:                       3.093   Cond. No.                     4.03e+03
==============================================================================
...
Notes:
[1] Standard Errors assume that the covariance matrix of the errors is correctly specified.
[2] The condition number is large, 4.03e+03. This might indicate that there are
strong multicollinearity or other numerical problems.

My model is looking at the number of slots available at a station and the corresponding ratings, distance, and total slots at the station.

According to my model, there is a signifant correlation between distance from yelp and whether there are less free bikes. There is an expected decrease of 0.0047 slots available distance. 

The only really signifant outcome from this model is the slots.1 value. If there are more slots, the number of free bikes increases by .4715. This is not surprising but good data.



## Challenges 
Foursquare had a lot of blank data which made it difficult to hold onto a lot of their input. 

The biggest challenge wasn't the code but getting a handle on the data and making sure that what I wanted to come in was coming in. I really struggled with keeping all of the data straight. Not having a lot of time with modelling and then jumping into the project was very difficult.

The API call build was challenging at first but once I got the call right, I didn't have to keep making calls and it was fine. 
## Future Goals
If I had more time and brain power, I would have spent more time on figuring out the stretch activity. 
