# Citi Bike Analytics - Jersey City 2018 - 2020

### Objective

The purpose of this project was to aggregate data found in the City Bike History Logs and find several interesting insights from data.

These designed visualizations were used to assemble dashboards and finally our Story.

 

### Data Source

The data is collected from the files found in the [Citi Bike Data](https://www.citibikenyc.com/system-data) webpage. 

Jersey City trip histories files from 2018 to 2020 were downloaded (30 files).

The files were then joined with Pandas to one dataframe. geopy library was used to calculate geographical distance between start stations and end stations. At the end the dataframe was saved to a csv file to be used in Tableau.



### Data Analysis

#### Trips (rides) breakdown

- Return trips (the same start and end station) are almost 6% of all trips. A half of them were done in  2020, probably impacted by COVID-19.
- Liberty Light Rail is (3192) the station with the most return trips.
- Median trip duration is between 5 - 10 minutes, but there are some outliers with trips lasting several days.

#### Time Distribution of Rides

- All three charts are showing two daily peaks, one for each rush hour.
- We can also see that ridership on weekends starts around 9:00 AM and it is much lower. As expected, more ridership during summer months than during winter months.

#### Gender Breakdown

- Majority of riders are male (~ 2/3). Females are riding in average slightly longer than males.
- Unknown riders are riding in average 3 - 4 time longer than males and females.
- There is no difference in ridership pattern over time among these 3 categories.

#### Age Breakdown

- Most active riders are between 30 and 40 years old, and very few are younger than 20.
- Percentage of riders between 50 and 60 years suddenly increased in 2020, Was that caused by COVID-19??
- Ridership pattern over time is the same for all age groups.

#### User Type Breakdown

- Majority of riders are "Subscribers". That is the same for all monitored quarters except for Q2 2020. The percentage of "Customer" is now slightly lower than for "Subscribers". It seems again one of COVID-19 impacts.
- The ridership pattern over time is the same for both categories.

#### Bike Utilization and Maintenance

- During the researched period of time there were 1,836 bikes in use.
- The bike ID # 26155 has the highest mileage (2,291) of all bikes and the most number of trips (1993).

#### Start Stations

- Stations that are closer to public transport systems tend to be more popular.
- Grove St PATH is the station with the highest number of rides.

#### End Stations

- The same as for the start stations, the end stations that are closer to public transport systems have most number of rides.
- Grove St PATH is again the station with the highest number of rides.
- Majority of rides end in Jersey City, but there are some people who go pretty far into NYC. This is why majority of end stations are in NYC.
- There are 185 end stations listed during the researched period and 89 of them have only 1 or 2 rides, and they are mostly in NYC

#### COVID-19 Impact

COVID-19 has rapidly affected our day to day life. In this analysis we have noticed many signs of that. Let's just mention a few of them.

- We can see a huge increase in a number of return trips in 2020. That could be explained by people not commuting.
- Similarly, from the "Trip Duration" chart we notice a peak in median trip duration. 
- The chart "Ridership over Months" displays a decrease in the ridership around April,as we could expect due to spring lockdown. 
- From "Top Hour" and "Distribution of Trips" charts, we can see that there is no morning peak in ridership in Q2 2020. Probably caused by closed businesses during that time. People are riding later in a day and mostly for leisure.



### Tableau

The following Tableau features I used during this project:

##### Combined Fields:

Start St. Id --> End St. Id 

Start Station Name --> End Station Name



##### Calculated Fields:

Avg. Distance per Bike

Geodistance (miles)

Number of Bikes

Number of Trips

Percent of Total

Rank

Top 10 - Bottom 10

Trip Distance

Trip Duration (min.)

Tripduration Aggregations



##### Parameters:

Select Aggregation









