# World Weather Analysis Challenge 
- Challenge #6. 
- Add the weather description to the weather data you’ve already retrieved in this module. 
- Use input statements to filter the data for their weather preferences, *which will be used to identify potential travel destinations and nearby hotels.*
- Choose four cities to create a travel itinerary. 
- Create a travel route between the four cities as well as a marker layer map.

## Overview of the Analysis
This new assignment consists of three technical analyses. You will submit the following deliverables:
1. Deliverable 1: Retrieve Weather Data.
2. Deliverable 2: Create a Customer Travel Destinations Map.
3. Deliverable 3: Create a Travel Itinerary Map.

## Analysis
# Deliverable 1: Retrieve Weather Data
- Obtain 2,000 random latitudes and longitudes.
- Get data for the closed city to these locations.
* Only 779 of the 2,000 requests were found, this makes a lot of sense since 70% of our planet is water.
- Perform an API call to get weather information from Open Weather by using the following URL:
*"http://api.openweathermap.org/data/2.5/weather?units=Imperial&APPID=" + api_key*
- Obtain the following weather data on the previously selected cities:
1. Lat.
2. Lng.
3. Max Temp.
4. Humidity.
5. Cloudiness.
6. Wind Speed.
7. Current Description (new addition).
- Only 721 of the 779 cities returned data.
- The resulted data is saved as "WeatherPy_Database.csv"

![Weather Database](https://user-images.githubusercontent.com/95668609/152660424-8aadb6be-83eb-49f5-a5ad-1a174769fa9a.png)


# Deliverable 2: Create a Customer Travel Destinations Map
- Prompt the user to enter a minimum and maximum temperature criteria.
- Based on the customer preferences I built a new DF with the desired cities available with the desired temperature.
- Perform an API call to get Hotel information from Google Nearby Search by using the following URL:
*""https://maps.googleapis.com/maps/api/place/nearbysearch/json" + params*
- Removed the Null Values.
- Create a marker layer for each desired city in a Google map.

![Vacation Selection](https://user-images.githubusercontent.com/95668609/152660429-5e1f8f55-1811-4aa2-8bae-1aac62833231.png)


# Deliverable 3: Create a Travel Itinerary Map
- I tested the platform a created a travel itinerary.
- My temperature selection was:
* What is the minimum temperature you would like for your trip? 55
* What is the maximum temperature you would like for your trip? 75
- My US cities selection were:
* King City
* Pacific Grove
* Laguna
* El Dorado
- Create a travel itinerary.

![Vacation Itinerary](https://user-images.githubusercontent.com/95668609/152660436-03006cae-5786-4a1d-95a5-36ae95298307.png)

