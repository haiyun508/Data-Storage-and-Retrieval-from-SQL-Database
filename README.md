# sqlalchemy_challenge
Congratulations! You've decided to treat yourself to a long holiday vacation in Honolulu, Hawaii! To help with your trip planning, you need to do some climate analysis on the area. The following outlines what you need to do.

# Step 1 - Climate Analysis and Exploration
To begin, use Python and SQLAlchemy to do basic climate analysis and data exploration of your climate database. All of the following analysis should be completed using SQLAlchemy ORM queries, Pandas, and Matplotlib.

## Precipitation Analysis

## Station Analysis

# Step 2 - Climate App



# Bonus: Other Recommended Analyses

## Temperature Analysis I


Hawaii is reputed to enjoy mild weather all year. Is there a meaningful difference between the temperature in, for example, June and December?


Use pandas to perform this portion.


Convert the date column format from string to datetime.


Set the date column as the DataFrame index


Drop the date column




Identify the average temperature in June at all stations across all available years in the dataset. Do the same for December temperature.


Use the t-test to determine whether the difference in the means, if any, is statistically significant. Will you use a paired t-test, or an unpaired t-test? Why?



## Temperature Analysis II


You are looking to take a trip from August first to August seventh of this year, but are worried that the weather will be less than ideal. Using historical data in the dataset find out what the temperature has previously looked like.


The starter notebook contains a function called calc_temps that will accept a start date and end date in the format %Y-%m-%d. The function will return the minimum, average, and maximum temperatures for that range of dates.


Use the calc_temps function to calculate the min, avg, and max temperatures for your trip using the matching dates from a previous year (i.e., use "2017-08-01").


Plot the min, avg, and max temperature from your previous query as a bar chart.


Use "Trip Avg Temp" as the title.


Use the average temperature as the bar height (y value).


Use the peak-to-peak (TMAX-TMIN) value as the y error bar (YERR).






## Daily Rainfall Average

Calculate the rainfall per weather station using the previous year's matching dates.

Sort this in descending order by precipitation amount and list the station, name, latitude, longitude, and elevation.



Calculate the daily normals. Normals are the averages for the min, avg, and max temperatures. You are provided with a function called daily_normals that will calculate the daily normals for a specific date. This date string will be in the format %m-%d. Be sure to use all historic TOBS that match that date string.


Set the start and end date of the trip.


Use the date to create a range of dates.


Strip off the year and save a list of strings in the format %m-%d.


Use the daily_normals function to calculate the normals for each date string and append the results to a list called normals.




Load the list of daily normals into a Pandas DataFrame and set the index equal to the date.


Use Pandas to plot an area plot (stacked=False) for the daily normals.


