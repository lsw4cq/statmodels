# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
The goal was to find a correlation between bike availability and being near office buildings and/or bars

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
6. Checked for duplicates
    * Duplicates were found. The only difference between the duplicates was the distance from the station so all were eliminated and distance can no longer be used reliably as a method of analysis for the Yelp data.

## Results
I found that there might be a correlation between yelp rating and free bikes but honestly I think it's a fluke since there aren't a lot of free bikes and it's random. Working with such a small dataset doesn't give way for good data. 

I also learned that getting the data into a state to be analyzed is signifcant.

## Challenges 
Yelp's categories does not include a generic office category so I used various other categories to try and collect that same data as foursquare. 

The biggest challenge wasn't the code but getting a handle on the data and making sure that what I wanted to come in was coming in. I really struggled with keeping all of the data straight and making sure that I wasn't making too many API calls.
## Future Goals
If I had more time I would have used a different city. I realized once I had been working on the project for awhile that the bike data wasn't awesome for what I wanted to look at and see.
