# Unit-6-Homework-Assignment
## Pythonic Monopoly 
In this assignment, we use Toronto neighbourhood data from Canada's 2001, 2006, 2011 and 2016 censuses to visualize (1) the evolution of dwelling types, (2) the evolution of average monthly shelter costs for owned vs. rented homes, (3) the progression of average house values, (4) the progression of average house values filtered by neighbourhood, (5) the progression of dwelling types filtered by neighbourhood,  (6) the top 10 most expensive neighbourhoods in 2016 with their average house prices over the four census observations, (7) the average house values by neighbourhood using a mapbox function, and (8) the average house prices by neighbourhood using a bar chart row facet. 

## Rental Analysis Notebook 
* Ln 1-3: We import our libraries, load our environment and APIs and read in the Census and GPS csv files, culminating in a dataframe called to_data. 
* Ln 4-7: Using the dataframe above, we define a function to create bar charts for the years 2001, 2006, 2011, and 2016, and create those charts.  
* Ln 8-10: Similarly, we create a new df called avg_monthly_costs, then create a function to visualize two line charts for monthly housing costs on owned vs. rented homes (using the information contained in the new df). 
* Ln 11-14: We calculate and plot average house values per year, then create a dataframe (from the to_data df) containing average house value by neighbourhood for the 4 census years. We then use hvplot to create an interactive chart that allows us to view average house value progression when filtering from the neighbourhood dropdown list.   
* Ln 15-16: We collect the data for all dwelling types by year (again filtering to_data) and create a bar chart showing the progression of dwelling types by neighbourhood, which users can choose from the dropdown list. The progression of dwelling types reflects the 2001, 2006, 2011 and 2016 censuses. 
* Ln 17-18: We obtain the data of the 10 most expensive neighbourhoods in 2016, and create a bar chart (using average house prices across the 4 censuses). 
* Ln 19-22 : We load neighbourhoods' GPS coordinates from the second .csv file, create a df of average house values for each neighbourhood, and merge the average values by neighbourhood with the GPS coordinates.   We then set up our matplot that allows us to choose neighbourhoods on a map of Toronto, with the darkest colours representing the most expensive neighbourhoods based on average census prices from 2001, 2006, 2011 and 2016 . 
* Ln 23: Using average house values by neighbourhood (same date in Ln 19-22) we create a bar chart row facet to plot house values by neighbourhood in the 2001, 2006, 2011 and 2016 censuses. 

## Dashboard notebook
In this notebook we, import the relevant libraries, initialize the panel extension, import the . csv files from the Rental Analysis notebook, obtain the data we used for our plots in the previous notebook, and create functions for panels (that will contain the plots above). We finish this notebook by creating a dashboard title, defining a welcome text, and setting the appropriate tab layout. 


### Note
To view visualizations, please refer to the .pdf versions of the Dashboard notebook and the Rental Analysis files. For the mapbox plot and different dashboard tabs , please refer to the .pdf called mapbox.pdf. 
