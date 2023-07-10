# python_api_challenge
WeatherPy
---------
### Background ###
A Python script to visualize the weather of over 500 cities of varying distances from the equator, that answers the overall quation: "What happens as you get closer to the equator?" This script uses the [citipy Python library](https://pypi.org/project/citipy/) and the [OpenWeatherMapAPI](https://openweathermap.org/api).

#### Objective ####
Create Plots to Showcase the Relationship Between Weather Variables and Latitude:
* Use the OpenWeatherMap API to retrieve weather data from the cities list
* create a series of scatter plots to showcase the following relationships:
  * Latitude vs. Temperature
  * Latitude vs. Humidity
  * Latitude vs. Cloudiness
  * Latitude vs. Wind Speed
* Compute Linear Regression for Each Relationship and overlay onto the scatter plots
  * Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude)
  * Analyze each plot and state the findings
 
<img width="615" alt="Screenshot 2023-07-09 at 7 12 21 PM" src="https://github.com/m-janssens-boop/python_api_challenge/assets/127706155/783d01f7-9322-4449-a6c4-8a34b7f7f377">

VacationPy
---------
### Background ###
A Python script to visualize ideal vacation destinations using the data compiled in WeatherPy. This script uses the Geoapify API and the geoViews Python library to create map visualizations.

#### Objective ####
* Create a map that displays a point for every city from WeatherPy, with the size of the point representing the humidity in each city
<img width="776" alt="Screenshot 2023-07-09 at 7 15 55 PM" src="https://github.com/m-janssens-boop/python_api_challenge/assets/127706155/09287a3f-749a-4314-bb03-a8ab1a0a8acc">

* Select an ideal weather climate and filter the data to only find locations that meet the given criteria
* Use this criteria to:
  * Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity
  * For each city, use the Geoapify API to find the first hotel located within 10,000 meters of the coordinates
  * Add the hotel name and the country as additional information in the hover message for each city on the map
<img width="717" alt="Screenshot 2023-07-09 at 7 16 48 PM" src="https://github.com/m-janssens-boop/python_api_challenge/assets/127706155/c47566cf-d1e9-4808-8bfb-33d8d80eb215">
