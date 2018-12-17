# WeatherPy - What's the Weather Like?

## Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter..."_

But, if pressed, how would you **prove** it?

![Equator](Images/equatorsign.png)

## WeatherPy

In this assignment I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. 
To accomplish this, I utilised the following: 
* [Citipy Python library](https://pypi.python.org/pypi/citipy), 
* [OpenWeatherMap API](https://openweathermap.org/api), and 
* A little common sense to create a representative model of weather across world cities.

Our objective is to build a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Final notebook consists of:

* Randomly select **at least** 500 unique (non-repeat) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed with the city number and city name.
* Save both a CSV of all data retrieved and png images for each scatter plot.

# Data Analysis:

1. **Temperature**: The temperature tends to increase towards the equator (Latitude=0), there are certain outliers between latitude (20 to 40) but that can be attributed to other environmental factors.
2. **Humidity**: For cities whose latitude lies between(-20 to 20), we observe that the humidity is very high(more than 60%).
3. **Cloudiness**: Based on the data Cloudiness and Latitude cannot be correlated.  
4. **Wind Speed**: The wind speed is very low for cities that lie in the latitude range of (-40 to 70).

