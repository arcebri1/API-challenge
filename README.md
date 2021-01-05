# Weather Data Analysis - API Calls

- - -

I analyzed the weather of at least 500 unique cities based on latitude and longitude using a series of successive API calls.
As well as created a heat map that displayed the humidity for every city.

- - -

## WeatherPy

Created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. This was accomplished by utilizing a [simple Python library](https://pypi.python.org/pypi/citipy), and [OpenWeatherMap API](https://openweathermap.org/api).

Created a series of scatter plots to showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude


Ran linear regressions on each relationship, separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude


### VacationPy

I used jupyter-gmaps and the Google Places API to:

* Create a heat map that displays the humidity for every city from the WeatherPy

* Narrowed down the DataFrame to find the ideal weather condition. For example:

  * A max temperature lower than 80 degrees but higher than 75.

  * Wind speed less than 5 mph.

  * Zero cloudiness.

  * Drop any rows that don't contain all three conditions.

* Used Google Places API to find the first hotel for each city located within 5000 meters of the coordinates.

* Plotted the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.


- - -
The data is provided by UCSD Extension: Data Science and Visualization Bootcamp.
- - -

Contact:

Email: arcebri1@gmail.com