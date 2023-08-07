# Cyclistic-Case-Study
In this case study I assume the role of a data analyst in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The executives believe the future sucess of the company depends on maximizing the number of Subscribers. I will be using a the data across the entire year of 2018 to further understand the differences between subscribers and customers and make informed reccomendations to executives. 
## Scenario 
Cyclistic Bike-Share is a Chicago based bike-share company that has two types of customers. It has three options for customers to choose from: single-ride passes, full-day passes, and annual memberships. Cyclistic considers riders that have annual passes to be members. While single-ride and full-day pass users are customers. Financial analysts with Cyclictic have concluded that members are much more profitable than regular customers. Due to this the executives believe that focusing on increasing members is the most important thing for Cyclistic's success moving forward.
## Defining-the-problem
The main problem the director of marketing is trying to focus on is increasing the number of members for Cyclistic. The main points that guide the future marketing program to this goal are the difference's between casual riders and members, why casual riders would become members and how can digital media influence casual riders to become members. However for this anaysis we will focus on the differences between casual riders and members. Though looking at the data we will be able to get an overview of patterns and correlations between these types of users and the data. learning how they differ will be helpful for marketing and executives teams in how they should market to casual users and how they can maximize memberships. 

# Business-task
## analyze historical bike trip data to determine how casual riders and members use Cyclistic bikes differently
## Data-sources  
The data being used in this case study is Cyclistic's historical trip data. This data has been made available by Motivate Interational inc. under this license (https://www.divvybikes.com/data-license-agreement). This is public data that explores all relevant ride trip info including ride_id, start_time, end_time, start_station_name, end_station_nam, start_lat, start_lng, end_lat, end_lng, usertype. It is worth noting that the data-privacy issues prohibit the use of riders personally identfiable infromations which means it will not tell us if casual riders are visiting from out of the area or if they are repeat users. 
## Data_cleaning
To begin the data was downloaded via 4 zip files then unzipped and stored in excel as csv files. I then began cleaning and manipualting the data in the following ways for all 4 files. 
* Created new columns and calculated start_time, end_time, ride_date, ride_time, day_of_week, ride_month
  * start_time and end_time were then formated as TIME HH:MM:SS
  * ride_date was formated as m/d/y
  * day_of_week was structured as NUMBER with no decimals 1-7
    * 1 = Sunday 7 = Saturday
  * ride_month structures as NUMBER with no decimals 1-12
  *  
## BigQuery SQL
Due to the size of the datasets I decided to move them to an analysis tool better suited for the task at hand for this I chose to use SQL via BigQuery.
After uploading all the data I began cleaning and transforming the data further. 
