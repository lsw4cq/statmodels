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
According to my model, there is a signifant correlation between ratings from yelp and foursquare and whether there are free bikes available. This can be seen in the low p-value. 

The r squared value is quite low. This means that as a whole my model isn't really going to be accurate. 

There is no correlation between available bikes and schools. Which is not surprising since most school kids don't share their bikes.

I tried to change the model into a regression model using Logistic regression but the varying amount of rows that were schools vs bars made the model unusable. 

## Challenges 
Foursquare had a lot of blank data which made it difficult to hold onto a lot of their input. 

The biggest challenge wasn't the code but getting a handle on the data and making sure that what I wanted to come in was coming in. I really struggled with keeping all of the data straight.

The API call build was challenging at first but once I got the call right, I didn't have to keep making calls and it was fine. 
## Future Goals
If I had more time and brain power, I would have spent more time on figuring out the stretch activity. 
