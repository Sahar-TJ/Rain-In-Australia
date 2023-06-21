# Rain-In-Australia

Australia is a country that is well-known for its diverse landscapes and weather patterns. One of the most significant weather phenomena that affect the country is rainfall. Rainfall in Australia varies significantly by region and season, making it a crucial factor for various industries, including agriculture, tourism, and infrastructure development.

In this project, we will explore the patterns and trends of rainfall in Australia, analyzing the historical data to understand the variations in rainfall across different regions and seasons. The objective of this project is to provide a comprehensive understanding of rainfall in Australia. We will be predicting if it will rain or no the following day. So our Target Variable is RainTomorrow

## Dataset Description

The dataset in this project is collected from [Kaggle](https://www.kaggle.com/datasets/jsphyg/weather-dataset-rattle-package). The dataset contains the data of rainfall from 2007 to 2017. It stores the rainfall patterns of various cities of Australia. There are 23 features in the data.

**Columns:**
- __Date:__ The date of observation
- __Location:__ The common name of the location of the weather station
- __MinTemp:__ The minimum temperature in degrees celsius
- __MaxTemp:__ The maximum temperature in degrees celsius
- __Rainfall:__ The amount of rainfall recorded for the day in mm
- __Evaporation:__ The so-called Class A pan evaporation (mm) in the 24 hours to 9am
- __Sunshine:__ The number of hours of bright sunshine in the day.
- __WindGustDir:__ The direction of the strongest wind gust in the 24 hours to midnight
- __WindGustSpeed:__ The speed (km/h) of the strongest wind gust in the 24 hours to midnight
- __WindDir9am:__ Direction of the wind at 9am
- __WindDir3pm:__ Direction of the wind at 3pm
- __WindSpeed9am:__ Wind speed (km/hr) averaged over 10 minutes prior to 9am
- __WindSpeed3pm:__ Wind speed (km/hr) averaged over 10 minutes prior to 3pm
- __Humidity9am:__ Humidity (percent) at 9am
- __Humidity3pm:__ Humidity (percent) at 3pm
- __Pressure9am:__ Atmospheric pressure (hpa) reduced to mean sea level at 9am
- __Pressure3pm:__ Atmospheric pressure (hpa) reduced to mean sea level at 3pm
- __Cloud9am:__ Fraction of sky obscured by cloud at 9am. ***
- __Cloud3pm:__ Fraction of sky obscured by cloud (in "oktas": eighths) at 3pm. See Cload9am for a description of the values
- __Temp9am:__ Temperature (degrees C) at 9am
- __Temp3pm:__ Temperature (degrees C) at 3pm
- __RainToday:__ Boolean: 1 if precipitation (mm) in the 24 hours to 9am exceeds 1mm, otherwise 0
- __RainTomorrow:__ The amount of next day rain in mm. Used to create response variable RainTomorrow. A kind of measure of the "risk".


*** _This is measured in "oktas", which are a unit of eigths. It records how many eigths of the sky are obscured by cloud. A 0 measure indicates completely clear sky whilst an 8 indicates that it is completely overcast._
