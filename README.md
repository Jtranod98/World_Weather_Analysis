# World_Weather_Analysis

APIs, google maps, pop-up markers, travel route

## Project Overview

Using APIs to collect and analyze weather data across cities worldwide.  PlanMyTrip will use the clients' weather preferences to recommend travel destinations and nearby hotels.

From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Using the Google Maps Directions API, create a travel route between the four cities and a marker layer map.

## Resources

- Software: Python 3.7, Jupyter Notebook, conda version 4.8.3, Pandas Library, SciPy, NumPy, Matplotlib 3.1.3
- Data Source: city_data.csv and ride_data.csv

## Methods

The analysis of the data was split into three stages:
Weather Database, Vacation Search, Vacation Itinerary

### Weather Database: collect the Data

  - Use the NumPy module to generate more than 2,000 random latitudes and longitudes.
  - Use the citipy module to list the nearest city to the latitudes and longitudes.
  - Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
  - Parse the JSON data from the API request.
  - Collect the following data from the JSON file and add it to a DataFrame:
  - City, country
  - Latitude and longitude
  - Maximum temperature
  - Humidity
  - Cloudiness
  - Wind speed
  - Weather description
  
### Vacation Search: create a map with pop-up markers that can display information on specific cities based on a customer's travel preferences.

  - Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
  - Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
  - Add pop-up markers to the map that display information about the city, current maximum temperature, and a hotel in the city.

###  Vacation Itinerary: visualize Travel Data
   
  - From the list of potential travel destinations,  four cities was randomly choosen to create a travel itinerary. 
  - Using the Google Maps Directions API,  a travel route was created between the four cities. 
  - A marker layer map was created with the four cities.
