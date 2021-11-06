# BootCamp-Mod-9-Surfs_Up
Performing analysis using SQLAlchemy on a SQLite database of weather data in Hawaii.

## Overview of Project

### Purpose
The purpose of this analysis is to use SQLAlchemy to sort weather data in a SQLite database to:
  1. determine if Oahu, Hawaii is a good place to open a surf and ice cream shop.
  2. put together a pitch to get investment backing.

## Analysis and Results
### Initial Queries
- The first step was to summarize the precipitation data on Oahu for the previous year.
  * The graph of the total precipitation per day seemed a little troubling since there were a few days per year where Oahu got a lot of rain. 
  * However, looking at the statistics, even though the max was almost 7 inches per day, the mean was close to 0 inches per day.
  * Low instances of rain is good for both a surfing shop and an ice cream shop.

<p align="center"><img src="https://github.com/M-Outlaw/BootCamp-Mod-9-Surfs_Up/blob/main/Graphics/Precip_Data.png"width="370" height="244"/>&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://github.com/M-Outlaw/BootCamp-Mod-9-Surfs_Up/blob/main/Graphics/precip_stats.png"width="271" height="149"/></p>

- Then, knowing that there are 9 weather stations collecting data on the island, it was important to see which station was most active.
<p align="center"><img src="https://github.com/M-Outlaw/BootCamp-Mod-9-Surfs_Up/blob/main/Graphics/Stations.png"width="186" height="147"/></p>

- After determining the most active weather station, all of the temperature data was pulled and used to create a frequency histogram to easily view the range of temperatures throughout the year.
  * The minimum temperature was 54 &deg;F.
  * The maximum temperature was 85 &deg;F.
  * The temperature on Oahu was most often around 75 &deg;F.
  
<p align="center"><img src="https://github.com/M-Outlaw/BootCamp-Mod-9-Surfs_Up/blob/main/Graphics/Temp_frequency.png"width="401" height="252"/></p>


### June and December Temperature Data
- Next, statistics were run for all of the June temperatures for all years of data and then the same for all of the December temperatures for all years.
  * The temperatures for December were very similar to those in June.
  * The mean temperature for June was 74.9 &deg;F and 71.0 &deg;F in December.
    - This shows that throughout the year there are only a few days that may be too cold for either surfing or ice cream.
  * The spread (standard deviation) of temperatures is small for both times of year, at 3.25 &deg; and 3.74 &deg.
    - This is also seen in the fact that the range for June is 21 &deg and December is 27&deg.
  * The maximum temperature in December was only 2 &deg lower than the maximum temperature in June.
  * The minimum temperature in December was only 8 &deg lower than the minimum temperature in June.

<p align="center"><img src="https://github.com/M-Outlaw/BootCamp-Mod-9-Surfs_Up/blob/main/Graphics/June_Temps.png"width="140" height="221"/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://github.com/M-Outlaw/BootCamp-Mod-9-Surfs_Up/blob/main/Graphics/Dec_Temps.png"width="159" height="221"/></p>

 
## Summary
### Oahu's Weather is Promising
- Based on the weather, Oahu seems to be a good place to set up a surf and ice cream shop.
  * The temperature is consistently good all year round.
  * There is minimal rain all year round.

### Additional Queries
- I would run the same statistical analysis done for June and December but for each month from each weather station to:
  * determine if there are any anomalies in the data. 
  * determine if there are locations on Oahu that have better weather conditions than others to set up a surf and ice cream shop.
- I would also run statistical analysis for all years on the precipitation during each month to:
  * confirm that the amount of rain is consistent from year to year.
  * determine if there is a month that is rainier than other months.
