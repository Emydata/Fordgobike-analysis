# Fordgobike Trip Data Exploration

## Dataset
The data contains information of 183,412 records of Fordgo bike trip in San Francisco. The dataset was made up of 16 columns and 183,412 rows. The columns are:
1. duration_sec
2. start_time
3. end_time
4. start_station_id
5. start_station_name
6. start_station_latitude
7. start_station_longitude
8. end_station_id
9. end_station_name
10. end_station_latitude
11. end_station_longitude
12. bike_id
13. user_type
14. member_birth_year
15. member_gender
16. bike_share_for_all_trip
The data set was downloaded from the udacity website for this project.

## Summary of Findings
In the exploratory analysis, I found that the highest trip duration was about 500secs, I also noticed that as trip duration increases the number of trips decreased showing a negative correlation. 
I went further to investigate other variables like member_age and discovered that users between age 20 and 50 rode for higher durations
than users from 60 years of age. Investigating the user_type variable, I found that customers used the bikes for longer durations than subscribers.
The service had higher number of rides between the hours of 8am and 9am and also between 5pm and 6pm on weekdays for both type of users.

## Key Insights for Presentation
For the presentation, my focus was on the ride duration and how other variables affect the duration  of the rides.
I started by plotting the distribution of the duration in minutes and found that the distribution has a long tail.
I used log transformation to plot the same distribution and discovered that there was a peak between 5 and 8 minutes, meaning that most of the rides took about 5 to 8 minutes. The average ride duration was 12 minutes and i also observed an  outlier 
which showed the maximum ride duration as 1424 minutes.

Investigating the hours of rides and the age group of members,I used seaborn to plot a countplot to group the ages, then I used seaborn catplot to plot the hourly rides per user type and age group.  
I found that the adult age group(30 to 50 years) had the highest number of trips between 8am to 9am and 4pm to 6pm on weekdays for both customers and subscribers.
The youth age group (19 to 30years) have the highest number of rides between 7pm and 11pm on weekdays for both subscribers and customers.

