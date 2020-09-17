## Wildfires in California and Daily Weather
Over the course of this project my team and I set out to search out data relating to wildfires in california, making use of web-based APIs to find data.


## Process 

It all started with a question, can one see any trends for a severity or likelihood of a fire started in local weather?

We managed to pull information about fires from 2013, 2015 and 2018 to compare directly to weather data on the exact date of the fire in the region where the fire was located.

Here we had to do some data clearning, a fairly large amount of the entries for the fires were incomplete, and locational data was simply not available. Additionally, many did not have an accurate end-date, listed simply as the end of the year the fire was recorded. To solve this, we shifted our scope to focus on the day the fire started.

![fire_data](Images\FireData.png)

Calfire served as the source for our fires, while the daily weather data was pulled from a service called OpenWeatherMap.

To start with, the data from the California fires was not available via an API, the Calfires data services were limited, but we were able to get information from the website itself using Chrome's browser information. From there, we were able to pull out data from the fires longitude and latitude and date using pandas, and could pull information for those specific dates and locations into the our jupyter notebook file.


## Findings

We set about making our comparisons, graphing fire information such as total area burned, date and location against weather information like wind speed, temperature and humidity.

![fire_data](Images\LocationGraph.png)

Altogether, we were somewhat surprised to find that windspeed seemed to be inversely proportional to likelihood of a fire breaking out, but it was difficult to find a real link to humidity and that same likelihood.

for illustrative purposes, we also created some maps in which all the fires within our data were logged year to year.

## Conclusions
The data around the specific weather conditions are not hard predictors of a fire, although the data does show somewhat higher likelihood on low-wind days, that doesnt relate to the total acreage burned, but further high winds could (and likely does) contribute to that in subsequent days of a fire.

