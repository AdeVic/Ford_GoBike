# (Dataset Exploration Title)
## by (your name here)


## Dataset

>This dataset includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area as at february 2019. It has a total of 183412 rows and 16 columns. The data is gotten from the 
it contains the following variables:

1.  duration_sec: How long was the ride in seconds 
2.  start_time: When the ride started
3.  end_time: When the ride ended
4.  start_station_id: The unique id for the station where the bike was picked for a ride
5.  start_station_name: The name of the station where the bike was picked for a ride
6.  start_station_latitude: The latitude of the station where the bike was picked for a ride
7.  start_station_longitude: The longitude of the station where the bike was picked for a ride
8.  end_station_id: The unique id for the station where the bike was dropped (where the ride ended)
9.  end_station_name: The name of the station where the bike was dropped (where the ride ended)
10. end_station_latitude: The latitude of the station where the bike was dropped (where the ride ended)
11. end_station_longitude: The longitude of the station where the bike was dropped (where the ride ended)
12. bike_id: The unique id of each bike
13. user_type: The categories of people that use the buke
14. member_birth_year: The year of birth for registered members/users
15. member_gender: The gender of registered members/users
16. bike_share_for_all_trip: Indicates whether the bike is used for alt trips or for last mile

## Required Software
Here, jupyter notebook is needed to run this analysis
The following libraries should be installed on the jupyter notebook
    * Pandas 
    * Numpy
    * Matplotlib
    * Seaborn

## List of files included in the project
The following files are in this project
    * README.md
    * Ford_GoBike_System_Part_I.ipynb
    * Ford_GoBike_System_Part_II.ipynb
    * 201902_fordgobike_tripdata.csv
    * Ford_GoBike_System_Part_I.html
    * Ford_GoBike_System_Part_II.slides.html


## Data Cleaning 
* Age_range variable was introduced using pd.cut() method which generated seven age_range which are: 80, 70, 60, 50, 40, 30, 20

* start_time, end_time, start_station_latitude, start_station_longitude, end_station_latitude, end_station_longitude and bike_id are recognized as unnecessary for this analysis and therefore were dropped 

* Some rows were missing and therefore were dropped because the dataset does not provide clues on how those can be filled. for instance a missing start station cannot be retrieved in this dataset
* duration_sec and member_birth_year came as object type but were changed to integer for better analysis
member_gender, 
* bike_share_for_all_trip were chnges and user_type from object data type to category

## Summary of Findings

> Customer user type trips take a longer duration compared to subscriber user type.
> Most trips takes an average of 500 seconds
> More than 90% of the trips are not shared for all trips. Therefore, they are majorly used as last mile means of transportation
> There are more subscribers and male in the dataset than customers, female and others
> Although there are less people in the age range of 60 but they tend to have more mean trip duration than others
> The male rider have lesser mean duration compared with other riders


## Key Insights for Presentation

> This analysis is focused majorly on the duration of ride, as this will be most important to the ride share industry.
>For the general population, the mean duration of ridearound 500 seconds, and most rides ranges between 280 to 800 seconds. The distribution of the ride is right skewed, showing that there are outliers on the right side; there are rides durations that are far higher than the normal.
> Among the different genders represented, the mean duration for the male is the lowest, although the male categoryy has the higher number of ride share users. Female and others have the same mean duration.
> Cstomers have longer trips than subscribers.
> The age_range variable vreated shows that people in their 60s have higher mean duration than others and their distribution is wide spread than others.
> Long ride is more common among the younger users than the elderly ones. We can also see that most frequent bike users are around age 20 to 45.


## Acknowledgements and credits
I will like to acknowledge ALX for giving the opportunity to gain this skill through Udacity
I will also like to thank Godswill Ayame the Session Lead and Obinna Iheanachor the Career Coach at Udacity for providing the neccesary assistance during this project.
GitHub resources, stackoverflow, and Kaggle has also been of a good help during the implementation of this analysis

## Bugs
The dataset provided does not contain enough detail to enable a time series data analysis which would have been an interesting kind of analysis in this project