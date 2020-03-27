# PyBer_Analysis
## Project Overview
The following analysis looks at PyBer's ride-sharing app data. For this analysis, the data was grouped according to city type (urban, suburban, and rural).

The following is the list of data visualizations that were delivered for the analysis of the PyBer ride-share app data:
* Bubble chart for all city types' ride-share data
* Box and whisker plots showing all city types for:
    * Ride count
    * Ride fare
    * Driver count
* Pie charts representing each city type's percentage of:
    * Total fares
    * Total rides
    * Total drivers

To further enhance the analysis, a summary-level data frame was created to show the following for each city type:
* Total rides
* Total drivers
* Total fares
* Average fare per ride
* Average fare per driver

Finally, a multiple-line plot for the sum of the fares for each city type was created.


## Resources
Data Source: city_data.csv, ride_data.csv Software: Python 3.7.6, Jupyter Lab 1.2.6 Libraries: Pandas, NumPy, Matplotlib, SciPy

## Analysis
### PyBer ride-share data for all city types (bubble chart)
The following bubble chart shows the ride-share data for all city types. Circle size correlates with number of drivers per city. The following observations can be gleaned from this visualization:
* Number of rides increases with city size (with rural cities having the lowest number of rides and urban having the highest)
* Number of drivers increases with city size (with rural cities having the lowest number of drivers and urban having the highest)
* Price per fare decreases with city size (with rural cities having the highest average fares and urban having the lowest)

![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/Fig1.png)

### PyBer ride count data for all city types (box and whisker)
The following box and whisker plot shows the ride count data for all city types. The following observations can be gleaned from this visualization:
* Number of rides increases with city size
    * The average number of rides in suburban cities is about 3.5 times higher than in rural cities
    * The average number of rides in urban cities is about 4 times higher than in rural cities
* In the urban city-type data there is one outlier

![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/Fig2.png)

### PyBer ride fare data for all city types (box and whisker)
The following box and whisker plot shows the ride fare data for all city types. The following observations can be gleaned from this visualization:
* Ride fare decreases with city size
    * The average fare of a ride in a rural city is $5 more per ride than in suburban cities
    * The average fare of a ride in a rural city is $11 more per ride than in urban cities
* There are no outliers

![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/Fig3.png)

### PyBer driver count data for all city types (box and whisker)
The following box and whisker plot shows the driver count data for all city types. The following observations can be gleaned from this visualization:
* Number of drivers increases with city size
    * On average, there are 4 times as many drivers in suburban cities than in rural cities
    * On average, there are 9 times as many drivers in urban cities than in rural cities
* There are no outliers

![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/Fig4.png)


### PyBer percentage of total fares data by city type (pie chart)
The following pie chart shows the percentage of the total fares each city type has. The following observations can be gleaned from this visualization:
* Percentage of the total fares increases with city size
    * Rural city fares represent the smallest portion of the total fares
    * Urban city fares represent the largest portion of the total fares

![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/Fig5.png)


### PyBer percentage of total rides data by city type (pie chart)
The following pie chart shows the percentage of the total rides each city type has. The following observations can be gleaned from this visualization:
* Percentage of the total number of rides increases with city size
    * The number of rural city rides represents the smallest portion of the total number of rides
    * The number of urban city rides represent the largest portion of the total number of rides

![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/Fig6.png)

### PyBer percentage of total drivers data by city type (pie chart)
The following pie chart shows the percentage of the total drivers each city type has. The following observations can be gleaned from this visualization:
* Percentage of the total number of drivers increases with city size
    * The number of rural city drivers represents the smallest portion of the total number of drivers
    * The number of urban city drivers represent the largest portion of the total number of drivers
* In comparison with the other pie charts which looked at total fares and total rides, the urban proportion of the total number is significantly larger.
![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/Fig7.png)

## Further analysis (Challenge)
### PyBer summary DataFrame
![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/DF1.png)

The DataFrame above confirms the observations gleaned from the data visualizations shown throughout this analysis.
* Total rides, total drivers, and total fares increase with city size
    * Rural cities have the lowest totals
    * Urban cities have the highest totals
* Average fares per driver and per ride decrease with city size
    * Rural cities have the highest averages
    * Urban cities have the lowest averages

Perhaps not as obvious from the other visualizations is the fact that the driver market is saturated.
* There are more total drivers than total rides in urban cities, meaning that not every driver actually completed a ride
* While there are more rides than drivers in suburban and rural cities, if the rides were divided equally, only some drivers would get 2 rides, while all others would only get 1 ride
* Being a PyBer driver therefore is not a lucrative way to earn a significant amount of money; however, it seems that the best opportunity would actually be in rural cities since the average fare per driver is highest there and the chances of getting to drive are highest as well
    

### Multiple-line plot for the sum of the fares for each city type
![](https://github.com/karenbennis/PyBer_Analysis/blob/master/analysis/Fig8.png)

The multiple-line plot for the sum of the fares for each city type above shows that a period of about 4 months, the sum of the fares is quite stable, with each city type's line not changing significantly over time.

While all 3 city times appeared to have a slight increase in fares in the third week of February 2019, the increase only seems noteworthy since all 3 city-types experienced it in the same week.

Between March and April, the urban cities' sums of fares go up and down from week to week, albeit, not dramatically. Perhaps there is another factor influencing this. Further analysis would be required to identify the cause of this behaviour. It may be useful to identify any sort of events which may have taken place for the weeks which had higher sums of fares.

Overall, the sum of the fares does not change dramatically throughout the entire time span; on any given week, the sum of the fares for urban cities was the highest, and the sum of the fares for rural cities was the lowest.
