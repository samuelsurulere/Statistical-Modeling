# Final-Project-Statistical-Modelling-with-Python

## Project/Goals

Make a get request to CityBikes API for bike stations. Choose a city covered by CityBikes API and extract location coordinates and number of bikes. Using the location of all the bike stations, extract information about specific POIs of interest (such as restaurants, bars and others) from the FOURSQUARE API and YELP API. Create a DataFrame and compare the results from both APIs to decide on which give more quality and relevant information (subjectively). Merge all three DataFrames into one and create an SQlite database from the DataFrames. Perform EDA and build a statistical model to under relationship between number of bikes and characteristics of respective POIs.

## Process
### Created the pull request function for each of the APIs. Created a DataFrame the city bikes, foursquare and yelp API calls for each preferred information that was extracted from the JSON object response. 
### Created an SQLite database using previous DataFrames and merged all three DataFrames into one for statistical analysis. 
### Performed exploratory data analysis process and visualized the data to make inference regarding possible relationships between variables. 
### Transformed and normalized the data.
### Built a statistical model, analyzed the results and provided valuable insights.

## Results
In comparing the quality of the responses from FOURSQUARE and YELP APIs, I initially posited that the data from YELP was more quality as it is very easy to understand and interpret the meaning of the numbers. But from the statistical perspective, the popularity index coefficient actually has a stronger positive influence on the number of bikes. Basically, the higher the popularity index, the more bikes available around that vicinity.

## Challenges 
I wasted a huge amount of precious time trying to figure out why my visualizations were strange and out-of-place. Only to discover that the DataFrames from my API were simply the repetitions of the first call made. Not spending enough time on the EDA process (especially data quality and data cleaning).

## Future Goals
Explore the city bikes API for city that has a really high number of bike stations. This will improve the accuracy of the model more.
Spend more time properly modifying the statistical model. I used brute-force in dealing with the outliers due to losing a huge amount of time to a bug.
Think on the logic to use the rating as a categorical variable and maybe classify the number of bikes into bins.
Reflect on the holistic meaning of the chosen variables used for the model. A deeper understanding of the variables and what they stand for will result to better analysis and deeper understanding of the statistical model.
