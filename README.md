# Travel Mapper

## Purpose
The purpose of this repository is to visualize travel locations on an interactive map using Folium and to create a time beam visualization of travel durations using Plotly. This allows users to easily see and explore various travel destinations based on their geographical coordinates and understand the duration of stays at each location.

## What This Repository Contains

1. **Travel Mapper Notebook**: 
   - A Jupyter Notebook that demonstrates how to load travel data, geocode locations, create an interactive map with Folium, and visualize travel durations with a time beam using Plotly.

2. **Data Files**:
   - `locations.csv`: The initial dataset containing travel locations with columns for departure/arrival status, timestamp, and location.
   - `locations_with_coordinates.csv`: The dataset augmented with latitude and longitude coordinates.

## How It Works

1. **Importing Libraries**: Import the necessary libraries, including Pandas for data handling, Folium for map visualization, and Plotly for creating interactive plots.

2. **Loading Data**: Read the CSV file containing the travel locations into a DataFrame using Pandas.

3. **Geocoding Locations and Data Preparation**: Use the geopy library to geocode the locations and obtain their latitude and longitude coordinates. Merge the geocoded coordinates with the original DataFrame and export the augmented data to a new CSV file.

4. **Map Creation, Adding Markers, and Display**: Using Folium, create an interactive map centered on the mean location of the provided coordinates. Add markers to the map with popups displaying the location names, customized to be flexible in width. The interactive map is then displayed.

5. **Data Preparation**: Prepare the data by calculating the duration of stay at each location.

6. **Time Beam Creation**: Use Plotly to create a bar chart where each bar represents the duration of stay at a location.

7. **Customizing the Visualization**: Customize the bars with labels and tooltips to provide more information.

8. **Displaying the Time Beam**: Display the time beam, showing an intuitive timeline of travel durations.

## Conclusion
In this notebook, I demonstrate how to visualize travel locations on an interactive map using Folium and how to create a time beam to represent the duration of stays at various locations using Plotly. These visualizations provide an intuitive way to explore travel data and understand travel patterns. The interactive map allows users to see the geographical spread of travel destinations, while the time beam offers a clear timeline of travel durations. This
