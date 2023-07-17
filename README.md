# Assignment-6-API
This is the challenge 6 with API being the main data source and the task is to display the results through geoapify

In this repository, there are several files in which are connected to the Assignment.
The two pythons: WeatherPy and VacationPy are the main source coding which uses Weather and Geoapify API to retrieve the real data and convert that data in a dataset in order to do some analyis.
The .gitignore file is used to 'ignore' one particular file for safety reason.
The folder 'output_data' refers to exporting the graphs from the python into an image and the dataset into a csv file.

To make this code work, you'll need API keys structured like:
geoapify_key = 'Add your API'
weather_api_key = 'Add you API'

The next step is to run the 'WeatherPy_Assigned_work.ipynb' first. This is because the API data gathering is from the WeatherPy which is then translated into a csv file for the seond code 'VacationPy'
as it uses the "read_csv" command to read the 'cities'.

As for which program needed to make it functional, the first code for both python files have all the import list which is needed.

What does the coding do?
In the 'WeatherPy' it extracts the raw data from the Weather API and collect the city data for coordination and statistic among all of the recorded cities. those series data are then converted into DataFrame
which is then used to present scatter plots based on various criterias. The second set is then used to find the regression line with the different hemispheres (North and South) as the main factors.

The second python, 'VactionPy' uses the cities.csv, exported from the first python file, to display the points of cities on a world map. the following sequences are used to narrow down ideal cities through filtering based on specific 'weather condition'. Then the list of 'ideal cities' are used to find the nearest hotel and add to the exisiting DataFrame. Then those detail are added to the world map as additional facts.
