# Plotly_Analysis
UT Module 12 Challenge

## Project Overview
Create a bellybutton diversity dashboard to identify 10 bacterial species in the bellybuttons of volunteers.  This dashboard will have a dropdown menu to show the details of the volunteer, a barchart showing the bacterial cultures found in their naval, a guage chart showing their washing frequency and a bubble chart of the bacterial cultures found in each sample. 

## Resources
Data Sources provided to analyze and minipulate included the samples.json file as well as utilizing the following software and applications:
- JavaScript
- HTML
- CSS
- Visual Studio
- Personal GitHub account

## Analysis and Workflow
The following flow was generated in our PyBer_Challenge_starter_code_final.ipynb (https://github.com/austin020269/PyBer_Analysis/blob/main/PyBer_Challenge_starter_code_final.ipynb) Jupyter Notebook file.

The ride share data frame was created by:
- retrieving the total number of rides, the total number of drivers and the sum of the fares for each city type.
- calculating the average fare per ride and average fare per driver for each city type.

![alt text](https://github.com/austin020269/PyBer_Analysis/blob/main/analysis/dataframe.PNG)

The mullti-line chart showing total fares for each city type was created by:
- creating a new dataframe showing the sum of the fares for each date.
- resetting the index on the dataframe.
- creating a pivot table with the date as the index, the columns ='type', and values='fare' to get total fares for each city.
- creating dataframe from the pivot table. 
- setting the "date" index to datetime datatype.
- creating a new dataFrame by week 'W' and get the sum of the fares for each week.
- plot the new dataframe using the df.plot() function. 

![alt text](https://github.com/austin020269/PyBer_Analysis/blob/main/analysis/Fig8.png)


## Summary

Some observations we can make about the pyber_summary_df dataframe include:
- there are more rides in urban cities than suburban or rural cities
- there are more drivers in urban cities
- fares and fares per ride are more expensive in rural cities, probably due to the length of the ride
- fares per ride are cheaper in urban cities

Some observations we can make from the Total Fare by City Type chart include: 
- the overall trends for each city type are relatively similar.
- their data never interesect each other
- an overall upward jump in fares in each city type in mid-February
- an overall upward trend in each city type in January
