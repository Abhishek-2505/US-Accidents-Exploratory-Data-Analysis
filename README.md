# US Accidents EDA : Project Overview
In case if the "US_Accidents_EDA(ori).ipynb" file is not opening [click here](https://colab.research.google.com/drive/1QSCa9lT2yHZGg9IL2CWxV1TT6T-pMnVk?authuser=1#scrollTo=zgKp7GnL94Ew).

## Workdone - Quick overview

- Collected the data from Kaggle, cleaned and handled all missing values.
- Gathered some insights like 

       - What are the states and cities with most and least number of accidents?
       - At what time do accidents occur most?
       - About the locations of the accidents.
       - What was the severity level of accidents? And the impact on traffic flow.
       - Different factors to consider during the accidents (like presence of traffic signal, junction etc.) 
         and also some natural factors (like temperature, period of day etc.).
 
## Resources used -
**Python Libraries** : Pandas, Numpy, Matplolib, Seaborn and Plotly.

**Datasets** : 
* US Accidents dataset - https://www.kaggle.com/sobhanmoosavi/us-accidents
* US States Dataset - https://www.kaggle.com/giodev11/usstates-dataset

**Platform used for execution** : Google colab

## Basic Analysis and Data Cleaning
After collecting the data, first thing need to be done is data cleaning. Here are some steps taken to clean the data.
* Converted datatype of the some columns which were not in proper format. 
* Deleted unwanted columns.

Missing values plot :

![Missing data heatmap](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/missing%20values%20heatmap.png)

* Handled all the missing values.



## Insights gathered...

### What are the states and cities with more number of accidents?
In this section we will analyze about the states and cities.

There are 51 states in USA but this data contains accident records of only 49 states. This analysis does not contain Alaska and Hawaii states.

Let's plot the statewise distribution of the accidents.
![Statewise distribution plot](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/newplot.png)
California is the state with most number of accidents which recorded 25.14% of accidents while South Dakota recorded 0.007% of accidents which is the least one.

Now let's analyze about the cities.

![Top 10 cities by accident](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/top%2010%20cities%20by%20accidents.png) ![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/city%20vs%20no%20of%20accidents.png)

Los Angeles is the city most number of accidents(2.35%) and Marble stands as least one with 0.000034% of accidents.
And also one thing to conider is 3668 cities recorded less than 5 accidents in those cities 1306 recorded only 1 accident in 4 years. 
This seems unusual, we may not have all the records from these cities.

We came to know about the statewise distribution of the accidents and also cities with most and least number of accidents. But what about the time? That is at what time most of the accidents took place. For getting that answer let's analyze about time.


### At what time do accidents occur most?

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/yearly%20ditribution%20of%20accidents.png)
Above plot shows the yearly distribution of the accidents from the year 2016 to 2020. This plot shows exponential growth in the rate of accidents from 2016 to 2020. But before making any conclusions it is better to know about the monthly distribution of these years.

Monthly distribution for the years 2016, 2017, 2018, 2019 and 2020 looks like
![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/monthly%20ditribution%20of%20the%20years%202016-20.png)

From this analysis we came to know that lot of data for the year 2016 is missing. 
So for yearly analysis it is better to consider from 2017 to 2020. The rate of increase in the accidents from 2017 to 2020 is 37.8%.

Now let's analyze about the daywise distribution of the accidents i.e which day has recorded more number of accidents and about the rate of growth in accidents from weekdays to weekends.
![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/daywise%20distribution.png)
The rate of accidents compared to weekdays decreases by 59.25% during the weekends.

Ok that's good! What about hourly distribution? Let's analyze it.
![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/hourly%20ditribution.png)
The rate of accidents increase from 5AM to 8AM and 2PM to 5PM exponentially while decreases from 6PM to 3AM gradually.

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/locations.png)
![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/location%20heatmap.png)

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/severity%20distribution.png)

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/accident%20duration.png)

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/taffic%20signal.png)

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/crossing-junction.png)

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/period%20of%20day.png)

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/weather%20condition.png)

![](https://github.com/Abhishek-2505/US-Accidents-Exploratory-Data-Analysis/blob/main/images/temperature%20distribution.png)

