# python-api-challenge
Module 6 API Challenge

In this deliverable, a Python script was created to visualize the weather of over 500 cities of varying distances from the equator. Using the citipy Python library Links to an external site, the OpenWeatherMap API Links to an external site, and problem-solving skills, a representative model of weather across cities has been created.

This project is divided into two parts: WeatherPy and VacationPy

WeatherPy:
To fulfill the first requirement, the OpenWeatherMap API was used to retrieve weather data from the cities list generated. Next, a series of scatter plots was created to showcase the following relationships:
Latitude vs. Temperature
Latitude vs. Humidity
Latitude vs. Cloudiness
Latitude vs. Wind Speed

To fulfill the second requirement, the linear regression for each relationship was computed. The plots were separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). 
Next, a series of scatter plots was created, being sure to include the linear regression line, the model's formula, and the r^2 values.

The following plots for WeatherPy were created:
Northern Hemisphere: Temperature vs. Latitude
Southern Hemisphere: Temperature vs. Latitude
Northern Hemisphere: Humidity vs. Latitude
Southern Hemisphere: Humidity vs. Latitude
Northern Hemisphere: Cloudiness vs. Latitude
Southern Hemisphere: Cloudiness vs. Latitude
Northern Hemisphere: Wind Speed vs. Latitude
Southern Hemisphere: Wind Speed vs. Latitude
After each pair of plots, the linear regression is modeling is explained, describing any relationships and findings that were uncovered (see summary).

VacationPy:
In this deliverable Jupyter notebooks, the geoViews Python library, and the Geoapify API were used. 
Main tasks are to use the Geoapify API and the geoViews Python library and Python to create map visualizations.
To start, a map that displays a point for every city in the city_data_df DataFrame was created, with the size of the point based on the humidity in each city.
Next, the city_data_df DataFrame was narrowed down to find the ideal weather condition for vacation. 
For example:
A max temperature lower than 27 degrees but higher than 21
Wind speed less than 4.5 m/s
Zero cloudiness
Next, a new DataFrame called hotel_df was created to store the city, country, coordinates, and humidity data.
For each city,  Geoapify API was used to find the first hotel located within 10,000 meters of the coordinates, then the hotel name and the country was added as additional information.

Summary of Findings:
Both the WeatherPy and VacationPy reveal a relationship between the latitue and longitude and the weather that can be expected. Though not exact, as can be seen in the scatter plot, the data can be helpful in determining how latitude and longitude relate to (and impact) cloudiness, humidity, wind speed and other conditions that one must prepare for. Using the data from WeatherPy, we can look at the conditions in a given city to see what the weather might be if we are planning a vacation. As mentioned in the document, longitude has a big impact on weather conditions, as does the topography of a given place. For example, the mountains in Patagonia, Argentina will be more like the mountains in Alaska, high in the Northern Hemisphere, while conditions close to the equator will be warmer and more temperate throughout the year. 

References:
The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 was provided.
