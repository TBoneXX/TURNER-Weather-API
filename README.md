# TURNER-Weather-API

## Location Search and Weather

This application takes a user entered location, calls the OpenWeather Geocoding API which returns the appropriate latitude and longitude coordinates.

The application then passes those coordinates to another API fetch which pulls the JSON data for the weather forecast for the current day and the following 5 days.

### Challenges

Currently the application is not functioning properly, and there are several issues contributing to these problems.

The first step in the process is to fetch the coordinates for the city, using the OpenWeather Geocoding API. This is necessary because the OpenWeather API that will deliver forecast data takes the latitude and longitude coordinates as an input.

For some unknown reason the Geocoding API is not returning usable data and is not responding properly to the API call, therefore this is causing the rest of the weather forecast data to not update properly rendering the app non-functional.

Because the Geocoding API is unable to be called from the application's code as it is, there is no lat/long to be passed to the forecast API.

Also, a significant issue that was not addressed was that the OneCall API is the designed API to used in this task, unfortunately OpenWeather has changed the access and pricing for this API, so we were unable to use it as prescribed in the assignment.

<img src="/App-image.png" title= "Weather App">