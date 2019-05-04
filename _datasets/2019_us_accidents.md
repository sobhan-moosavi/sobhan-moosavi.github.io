---
title: "US-Accidents: Countrywide Traffic Accident Dataset"
collection: datastes
permalink: /datasets/us_accidents
excerpt: This dataset contains country-wide motor-vehicle accidents data for 49 States of the US, which is continuously being collected from February 2016. Currently, there are more than 2.25 million accident records in this dataset. 
date: 2019-05-05
---

## Description 


## Acknowledgment
Please cite the following paper if you use this dataset:

* Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, and Rajiv Ramnath. ["A Countrywide Traffic Accident Dataset."](#), 2019. 

## Usage Policy and Legal Disclaimer
This dataset is being distributed only for __Research__ purposes, under [Creative Commons Attribution-Noncommercial-ShareAlike license (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/){:target="_blank"}. By clicking on download button(s) below, you are agreeing to use this data only for non-commercial, research, or academic applications. 


## Download
* __Version 1 (May 2019):__ In this version, we provide data which is collected from February 2016 to March 2019 for the [Contiguous United States](https://en.wikipedia.org/wiki/Contiguous_United_States){:target="_blank"}. In this set, we have about 2.25 million traffic accidents. Download data from [here](#){:target="_blank"}. 


## Coverage
The dataset covers 49 US States. Following diagram shows the current data distribution over all the states. 

## Format
The data is provided in terms of a __single CSV file__. Following table describes the data attributes: 

| \# | Attribute | Description | Nullable |
|:------:|:---------:|-------------|:--------:|
| 1 | ID | This is the unique identifier of the accident record | No |
| 2 | Source | Indicates the source of the accident which can be MapQuest, Bing, or both. | No |
| 3 | TMC | A traffic accident may have a [Traffic Message Channel (TMC)](https://wiki.openstreetmap.org/wiki/TMC/Event_Code_List){:target="_blank"} code which provides more detailed description of the event. | Yes |
| 4 | Severity | Shows the severity of the accident (a number between 1 and 4). | No |
| 5 | StartTime | Shows the start time of the accident in local time zone. | No |
| | EndTime | Shows the end time of the accident in local time zone. | No |
| | Start_Lat | Shows the latitude in GPS coordinate of start point. | No |
| | Start_Lng | Shows the longitude in GPS coordinate of start point. | No |
| | End_Lat | Shows the latitude in GPS coordinate of end point. | Yes |
| | End_Lng | Shows the longitude in GPS coordinate of end point. | Yes |
| | Distance (mi) | Shows the radius of impact. | No |
| | Description | Shows the natural language description of the accident. | No |
| | Number | Shows the street number in address field. | Yes |
| | Street | Shows the street name in address field.  | Yes |
| | Side | Shows the relative side of a street (R/L) in address field. | Yes |
| | City | Shows the city in address field. | Yes |
| | County | Shows the county in address field. | Yes |
| | State | Shows the state in address field. | Yes |
| | ZipCode | Shows the zipcode in address field. | Yes |
| | Country | Shows the country in address field. | Yes |
| | Timezone | Shows the timezone based on the location of an accident. | Yes |
| | AirportCode | Shows the closest weather station to the reported accident. | Yes |
| | W_Timestamp | Shows the timestamp of weather observation record in location time. ||
| | Temperature (F) | Shows the temparature in fahrenheit. ||
| | Wind_Chill (F) | Shows the wind chill in fahrenheit. ||
| | Humidity (%) | Shows the humidity in percentage. ||
| | Pressure (in) | Shows the air pressure in ??. ||
| | Visibility (mi) | Shows visibility in miles. ||
| | Wind_Direction | Shows wind direction.  ||
| | Wind_Speed (mph) | Shows wind speed in miles per hour. ||
| | Precipitation (in) | Shows precipitation amount in ??, if there is any. ||
| | Condition | Shows the weather condition (rain, snow, thunderstorm, fog, etc.) ||
| | Amenity | A POI annotation which indicates presense of [amenity](#) in a nearby location. | No |
| | Bump | A POI annotation which indicates presense of [bump](#) in a nearby location. | No |
| | Crossing | A POI annotation which indicates presense of [crossing](#) in a nearby location. | No |
| | Give_Way | A POI annotation which indicates presense of [given_way](#) in a nearby location. | No |
| | Junction | A POI annotation which indicates presense of [junction](#) in a nearby location. | No |
| | No_Exit| A POI annotation which indicates presense of [no_exit](#) in a nearby location. | No |
| | Railway | A POI annotation which indicates presense of [railway](#) in a nearby location. | No |
| | Roundabout | A POI annotation which indicates presense of [roundabout](#) in a nearby location. | No |
| | Station | A POI annotation which indicates presense of [station](#) in a nearby location. | No |
| | Stop | A POI annotation which indicates presense of [stop](#) in a nearby location. | No |
| | Traffic_Calming | A POI annotation which indicates presense of [traffic_calming](#) in a nearby location. | No |
| | Traffic_Signal | A POI annotation which indicates presense of [traffic_signal](#) in a nearby location. | No |
| | Turning_Loop | A POI annotation which indicates presense of [turning_loop](#) in a nearby location. | No |
| | Sunrise_Sunset | Shows the daylight condition (day or night) based on sunrise/sunset. | Yes |
| | Civil_Twilight | Shows the daylight condition (day or night) based on [civil twilight](#). | Yes |
| | Nautical_Twilight | Shows the daylight condition (day or night) based on [nautical twilight](#). | Yes |
| | Astronomical_Twilight | Shows the daylight condition (day or night) based on [astronomical twilight](#). | Yes |

## Applications of Dataset
US-Accidents can be used for numerous applications such as real-time accident prediction, studying accident hotspot locations, casualty analysis and extracting cause and effect rules to predict accidents, or studying the impact of precipitation or other environmental stimuli on accident occurrence. 
