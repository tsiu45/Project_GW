# Project_GW

Analysis and visualization of a geolocation time-series dataset
==================================================
Objective of this project is to explore the geolocation time-series dataset and extract out interesting driving-related information to display to a user.

GIS libraries I use are: **Folium, GeoPandas** and **Shapely**.
Map tiles are from **OpenStreetMaps**.
The codes are located in this file [Shift analysis.ipynb](https://github.com/tsiu45/Project_GW/blob/master/Shift%20analysis.ipynb). To view the fully rendered version including the resulting interactive maps, you can view it on **Jupyter nbviewer** [here](https://nbviewer.jupyter.org/github/tsiu45/Project_GW/blob/master/Shift%20analysis.ipynb).

Methodology:
----------------
Data is scrubbed and checked for consistency and resonableness. Secondary information such as longitudinal and lateral acceleration were derived from primary data.

As part of the exploratory data analysis, diagnotic charts were created to visualize the range and volatility of the data. Summary statistics were also generated to gauge the reasonableness of the data. Data was then grouped by different combinations of activity types and/or filtered by other indicators. Once a good understanding of the data was achieved, a final set of groupings was chosen for the final presentation of the result. Since the geolocation component of the result is very meaningful, the results are presented as visualizations on a set of interactive maps.

Result Summary:
--------------------
The final results are 4 sets of driving-related information visualized as layers on an interactive map:
1. Animated timestamped polyline plot to visualize vehicle location across timespan
2. Linear-colored polyline to visualize speed variations along route
3. Different activity types (in-vehicle vs on-foot) and traffic pattern (congestion vs high speed) are visualized as colored layers over the base map
4. Driving telematics such as hard braking, hard acceleration and hard cornering are extracted and visualized as colored layers over the base map
