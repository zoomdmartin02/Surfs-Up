# Surfs-Up
## Technology:  SQLite, SQL Alchemy & Flask
"SQLite is a software library that implements a self-contained, serverless, zero-configuration, transactional SQL database engine."  [www.tutorialspoint.com](https://www.tutorialspoint.com/sqlite/sqlite_overview.htm)

SQL Alchemy is the connectivity solution that connects a development environment to a SQLite database, exposing methods to query or manipulate databases.

Flask is a solution that allows for SQL Alchemy results to be rendered to a web page.

## Overview:  Surfing & Icecream
Our client would like to open a surf and icecream shop in Hawaii.  The client is targeting the island of Oahu, but is concerned about the weather patterns on this island and would like to know how much rainfall occurs and what the temeratures are at certain times of the year.  Our client has opened a shop like this before, but had a negative experience due to too much rainfall and cooler temperatures at a higher frequency.

We have been hired to provide analysis to determine the details of weather data on Oahu and confirm the suitability of the location.  Our data is a SQLite database.  We will be connecting to this database from Pandas through SQL Alchemy.  We will query the database for temperatures in June and December and summarize the data.

Once we have our data, we will convert it to a Pandas dataframe and then use the .describe() function to create summary data for our analysis.

## Results:  Temperatures in June and December on Oahu
Following are the results from our review of the June and December temperatures on Oahu:

![](/Resources/June_temps_summary.png)

![](/Resources/December_temps_summary.png)

bulleted list with three major points from the two analysis deliverables.  Use images
## Summary:  high-level summary of the results and two add'l queries that you would perform to gather more weather data for June and December.