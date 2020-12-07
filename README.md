# Surfs-Up
## Technology:  SQLite, SQL Alchemy & Flask
"SQLite is a software library that implements a self-contained, serverless, zero-configuration, transactional SQL database engine."  [www.tutorialspoint.com](https://www.tutorialspoint.com/sqlite/sqlite_overview.htm)

SQL Alchemy is the connectivity solution that connects a development environment to a SQLite database, exposing methods to query or manipulate databases.

Flask is a solution that allows for SQL Alchemy results to be rendered to a web page.

## Overview:  Surfing & Icecream
Our client would like to open a surf and icecream shop in Hawaii.  The client is targeting the island of Oahu, but is concerned about the weather patterns on this island and would like to know what the temeratures are at certain times of the year.  Our client has opened a shop like this before, but had a negative experience due to too much rainfall and cooler temperatures at a higher frequency.

We have been hired to provide analysis to determine the details of weather data on Oahu and confirm the suitability of the location.  Our data is a SQLite database.  We will be connecting to this database from Pandas through SQL Alchemy.  We will query the database for temperatures in June and December and summarize the data.

Once we have our data, we will convert it to a Pandas dataframe and then use the .describe() function to create summary data for our analysis.

## Results:  Temperatures in June and December on Oahu
Following are the results from our review of the June and December temperatures on Oahu:

![](/Resources/June_Temps_Summary.png)

![](/Resources/December_Temps_Summary.png)

A review of the data tells us that the range of data occurs between 2010 through 2016.  Across this range of time, there is an overall sample of 1700 measurments in the month of June and 1517 measurements occurring in the month of December.  The following points are noted from these descriptive statistics:

* At a cursory level, it appears from the summary statistical data that this location could be favorable to having a surf and icecream shop.  Max temps in June being 85 and average or mean temps being almost 75 all sound like good surfing and icecream weather.

In December, mean temperatures are 71, 4 degrees less than June sounds like the weather is a little cooler, but still seems like surf and icecream weather.  However, the minimum temp in December is 56 a bit cool.

* The mean and median (50th percentile) are both measures of central tendency.  When these numbers are similar, it usually indicates that the underlying data is symmetric or not skewed in eather direction.  Both in June and December, the mean and median are similar.

* The standard deviation measures the spread of data.  Data is normally considered symmetric if most of the observations are spread within e standard deviations of the mean.  June's standard deviation is 3.25.  3 standard deviations for June temps is 9.75.  June's mean is 74.94.  June's minimum temp is 64 which is a difference from the mean of 10.944.  Junes maximum temp is 85 and that makes a difference from the mean of 10.056.  June temps still appear to be symmetric but since there are some measurements outside 3 standard deviations, a deeper look might be needed.

December's standard deviation is 3.74592.  December's minimum temp is 56 and the max temp is 83.  The mean is 71.04.  Three standard deviations is 11.23.  The difference between the mean and the min temp i 15.04 and the difference from the max to the mean is 11.95.  So while the distribution is generally symtric, there could be some outliers on the bottom side.

For a pictorial view of the data in June and December, see the following plots:

![](/Resources/June_Temps.png)

![](/Resources/December_Temps.png)


bulleted list with three major points from the two analysis deliverables.  Use images
## Summary:  high-level summary of the results and two add'l queries that you would perform to gather more weather data for June and December.