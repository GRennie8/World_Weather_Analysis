# World Weather Analysis

## Overview of Analysis

Working with the PlanMyTrip app, I made a few changes to take the app to the next level. Specifically, adding the weather description to the weather data already retrieved in this module. I also added the ability for beta testers to use input statements to filter the data for their weather preferences, which will be used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will choose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, the user can create a travel route between the four cities.

## Summary

 - I created a set of 2000 random longitudess and latitudes using the code np.random.uniform.

![Screen Shot 2022-06-13 at 3 08 33 PM](https://user-images.githubusercontent.com/104115586/173445829-8fa8d491-c0e1-47cb-b435-7081efc1acad.png)

 - Using the 'citipy' module in Pandas, the coordinates were used to find the nearest city. If no city was found near to the random coordinates they were disregarded. The search yielded a total of 734 cities.


![Screen Shot 2022-06-13 at 3 12 45 PM](https://user-images.githubusercontent.com/104115586/173446381-ced1e9f0-67a4-43e9-b3b0-7f95db949055.png)

 - The user is prompted to input their preferred temperature at the destination. This information is used to create a new DataFrame with only cities within that temperature range.
- This map shows the cities found through citipy. I then added a pop up marker for each city. These markers display the hotel name, city, country and a weatehr description consisting of Max temp and a brief description of current weather conditions.

![WeatherPy_vacation_map](https://user-images.githubusercontent.com/104115586/173443678-6b848502-217b-4d88-979d-4d5016443329.png)

- This is an example of a possible travel itinerary in Spain and Portugal. It starts and ends in La Rioja, Spain (marker E).


<img width="990" alt="WeatherPy_travel_map" src="https://user-images.githubusercontent.com/104115586/173443656-400c5d44-cedc-4319-a8ef-ce3d96b3984a.png">

 - Pop up markers added to display hotel information and current weather description.


<img width="1661" alt="WeatherPy_travel_map_markers" src="https://user-images.githubusercontent.com/104115586/173443630-3b668ca1-cc67-4b1b-a466-c9ee6982bbb6.png">
