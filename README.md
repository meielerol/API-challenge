# API-challenge

Let's prove it gets hotter near the equator...

## WeatherPy

Assists in visualizing >500 cities across the world using randomly generated coordinates across the globe. This data is then paired with the closest city with a population >500 using the [citipy Python library](https://pypi.python.org/pypi/citipy). Utilized the [OpenWeatherMap API](https://openweathermap.org/api) to gather current weather data for the date the information is run.

Data files and figures are saved in the Output-Data file.

### Output-Data

- Contains the following:
    - csv file of randomly generated cities across the world
    - figures of the world comparing latitude to temperature, humidity, cloudiness, and wind speed
    - figures of the northern and southern hemispheres each comparing latitude to temperature, humidity, cloudiness, and wind speed with linear regression lines
    - figure of the data set latitude vs. longitude

## VacationPy

Based on the locations found in WeatherPy, this file assists in finding locations that meet specific vacation criteria and hotels within that area.

Vacation weather criteria:
- Between 70-80 degrees F
- Wind speed < 10 mph
- 0% cloudiness

Hotel criteria:
- Within 5000 meter radius
- Google API must return results for keyword and type "hotel"

## Notes:

OpenWeatherMap and Google Maps API keys are required to run these notebooks.

Please save your API keys in a python file named "api_keys.py". Below is the text that should go into this file, fill in the areas that say "YOUR KEY HERE" with the appropriate API keys for each application.

#OpenWeatherMap API Key

weather_api_key = "YOUR KEY HERE!"

#Google API Key

g_key = "YOUR KEY HERE!"