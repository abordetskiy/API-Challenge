# WeatherPy and VacationPy - Find your own sunshine and rainbows

### This project was incredibly rewarding as it rewarded me with a tool that I could use personally for my own goals. It implements several API pulls from OpenWeatherAPI and Google Maps API. 

#### Pulling in latitude and longitude, WeatherPy gets climate data and plots that data onto charts to first visualize the correlations globally, and then splits the same graph between Northern and Southern Hemispheres. These 'split' graphs include linear regression as and Pearson's correlation values. Detailed Analysis for each graph is included below the graph and should remain consistent between updated data (assuming global consistency of weather patterns). The general finding is intuitive, the farther away from the equator you get, the cooler the temperature.

#### Apart from pulling up a global humidity heatmap, VacationPy pulls the .csv file exported by WeatherPy and narrows that data based on artificial "perfect vacation" criteria. It then locates hotels within 5000 meters of those coordinates and plots them on the map to show the user which hotels on the planet match those "perfect vacation" criteria. My personal vacation centered around camping in a storm, so I chose windy, cloudy locations. The criteria in kernel 4 are fairly self explanatory and can be adjusted to the user's liking. 

###### Both .ipyng files includes an API Keys that are ignored by Git and supplied via a .env file. In order to run real-time data, please enter a valid api key, or import a CSV file. Directions for both options are in the .ipynb file comments.

Note: A very valuable skill gained in this project is the use of time.sleep() to pause the API pull so as to not exceed use per minute restrictions (and API key lockdown)