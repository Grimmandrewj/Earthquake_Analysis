# Goal
- In this assignment, I was tasked with assisting the USGS (United States Geological Survey) in creating a new set of tools allowing them to visualize their earthquake data
- I was to obtain a JSON file from the provided datasets located at https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php
- I was then to create an interactive visualization reflecting the data

# Method
- First, I selected the dataset and set the API endpoint as a variable
- I then created a function for setting the circle marker colors based on depth of the earthquake

![image](https://github.com/Grimmandrewj/Earthquake_Analysis/assets/120341249/436b42f6-0acc-40b0-a3e1-3448a4b498b7)

- I then created a function set to run for each feature in the array and provided each feature with a popup describing the location, time, magnitude, and depth of the earthquake
- I then created a GeoJSON layer containing the features array and ran the onEachFeature function for each piece of data in the array

![image](https://github.com/Grimmandrewj/Earthquake_Analysis/assets/120341249/c72b93db-e641-47f6-ab5d-3c7fb745f26c)

- I then sent the layer to the createMap function and created the base layers
- Then, I created the basemaps object to apply to the street map and an overlay object to contain the overlay
  
![image](https://github.com/Grimmandrewj/Earthquake_Analysis/assets/120341249/450a3f51-b9a9-48ee-b819-c8c1b162262b)

- I then created the map and the legend based on the returned data

# Summary and Results
- The data was successfully visualized and the popups display the appropriate data for each earthquake:

![image](https://user-images.githubusercontent.com/120341249/231945208-3dde068c-5399-49d5-a198-fa80abe5743f.png)

- The circle markers demonstrate magnitude and the color demonstrates depth
