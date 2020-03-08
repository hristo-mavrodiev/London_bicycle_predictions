# ML_Project
Machine learning course for Softuni 2019


# London Bike sharing demand predicton
## Machine learning algorithms for prediction of bike sharing demand in London.


## Author: Hristo Mavrodiev
Project requirements - [link](https://www.dropbox.com/s/yd458ut3qbo3tr0/assessment-guidelines.txt?dl=1)



![alt text](https://imgs.xkcd.com/comics/timeline_of_bicycle_design.png)
   
   XKCD.com



## The  Datasets description
The following code shows the loading of the bike sharing dataset. The data is gathered from 3 sources:  
 * https://cycling.data.tfl.gov.uk/ *'Contains OS data © Crown copyright and database rights 2016' and Geomni UK Map data © and database rights [2019] 'Powered by TfL Open Data'* - Bike sharing usage dataset
 * https://freemeteo.com - weather data
 * https://www.gov.uk/bank-holidays - official bank holidays in London.
 
 
After the data is grouped by hour and merged is published on "Kaggle" - 
https://www.kaggle.com/hmavrodiev/london-bike-sharing-dataset [1]  
*Note*: The official data for bike sharing contains "Start date" and "End Date" columns, for the calculations the trips are grouped by "Start date" column for every hour.So if the sharing is the long duration and passes 1 hour it's not  counted again.




### Metadata:
"timestamp" - *timestamp field for grouping the data*  
"cnt" - *the count of a new bike shares*  
"t1" - *real temperature in C*  
"t2" - *temperature in C "feels like"*  
"hum" - *humidity in percentage*  
"wind_speed" - *wind speed in km/h*  
"weather_code" - *category of the weather*  
"is_holiday" - *boolean field - 1 holiday / 0 non holiday*  
"is_weekend" - *boolean field - 1 if the day is weekend*   
"season" - *category field meteorological seasons: 0-spring ; 1-summer; 2-fall; 3-winter.*  

       
       
  


"weathe_code" category description:  
*1 = Clear ; mostly clear but have some values with haze/fog/patches of fog/ fog in vicinity  
2 = scattered clouds / few clouds  
3 = Broken clouds  
4 = Cloudy  
7 = Rain/ light Rain shower/ Light rain  
10 = rain with thunderstorm  
26 = snowfall  
94 = Freezing Fog*
