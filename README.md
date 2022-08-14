# python-api-challenge

## Part 1: WeatherPy

In this section, 500+ cities of varying distances from the equator were analyzed using a [simple Python library](https://pypi.python.org/pypi/citipy) and [OpenWeatherMap API](https://openweathermap.org/api) to create a representative model of weather across cities.

First, a series of scatter plots were created to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

Next, the linear regression for each relationship was computed. This time, the plots were separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude


## Part 2: VacationPy

First, a heat map displaying the humidity for every city from Part 1 was created. Then, the list of cities was narrowed to represent an ideal weather condition. 

  * A max temperature lower than 78 degrees but higher than 60.

  * Wind speed between 5 and 20 mph.

  * Zero cloudiness.

  * Less than 60% humidity.

  Each city that didn't satisfy all four conditions was dropped ensuring the weather conditions were ideal. Finally, Google Places API was used to find the nearest hotel for each city (within 5,000 meters) and they were plotted on top of the humidity heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**.

## Analysis

* In general, temperatures decrease as you move further away from the equator.
* The highest temperatures don't seem to be at the equator but slightly north, roughly 20 to 40 degrees latitude.
* In the Southern Hemisphere, wind speeds seem to decrease as you move closer to the equator. However, this is only a very slight correlation.
* Overall, temperature is the only metric that has a clear relationship when compared to latitude. When looking at humidity, cloudiness, and wind speed, latitude has little or no effect.

## Resources

* Module 6 Challenge Instructions
* OpenWeatherMap API
* Google Places API

