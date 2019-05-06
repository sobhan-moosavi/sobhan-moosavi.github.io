---
title: "US-Accidents: Countrywide Traffic Accident Dataset"
collection: datastes
permalink: /datasets/us_accidents
excerpt: This is a countrywide motor-vehicle crash dataset, which covers 49 states of the United States. The data is continuously being collected from February 2016. Currently, there are 2.25 million accident records in this dataset. Each accident record is described by 49 attributes including location, time, weather, etc. 
date: 2019-05-05
---

## Description 
This is a countrywide traffic accident dataset, which covers 49 states of the United States. The data is continuously being collected from February 2016, using several data providers, including two APIs which provide streaming traffic event data. These APIs broadcast traffic events captured by a variety of entities, such as the US and state departments of transportation, law enforcement agencies, traffic cameras, and traffic sensors within the road-networks. Currently, ther are 2.25 accident records in this dataset. For more detailed information about this dataset, please read below descriptions.

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
| 6 | EndTime | Shows the end time of the accident in local time zone. | No |
| 7 | Start_Lat | Shows the latitude in GPS coordinate of start point. | No |
| 8 | Start_Lng | Shows the longitude in GPS coordinate of start point. | No |
| 9 | End_Lat | Shows the latitude in GPS coordinate of end point. | Yes |
| 10 | End_Lng | Shows the longitude in GPS coordinate of end point. | Yes |
| 11 | Distance (mi) | Shows the radius of impact. | No |
| 12 | Description | Shows the natural language description of the accident. | No |
| 13 | Number | Shows the street number in address field. | Yes |
| 14 | Street | Shows the street name in address field.  | Yes |
| 15 | Side | Shows the relative side of a street (R/L) in address field. | Yes |
| 16 | City | Shows the city in address field. | Yes |
| 17 | County | Shows the county in address field. | Yes |
| 18 | State | Shows the state in address field. | Yes |
| 19 | ZipCode | Shows the zipcode in address field. | Yes |
| 20 | Country | Shows the country in address field. | Yes |
| 21 | Timezone | Shows the timezone based on the location of an accident. | Yes |
| 22 | AirportCode | Shows the closest weather station to the reported accident. | Yes |
| 23 | W_Timestamp | Shows the time-stamp of weather observation record in local time. ||
| 24 | Temperature (F) | Shows the temperature in Fahrenheit. ||
| 25 | Wind_Chill (F) | Shows the wind chill in Fahrenheit. ||
| 26 | Humidity (%) | Shows the humidity in percentage. ||
| 27 | Pressure (in) | Shows the air pressure in ??. ||
| 28 | Visibility (mi) | Shows visibility in miles. ||
| 29 | Wind_Direction | Shows wind direction.  ||
| 30 | Wind_Speed (mph) | Shows wind speed in miles per hour. ||
| 31 | Precipitation (in) | Shows precipitation amount in ??, if there is any. ||
| 32 | Condition | Shows the weather condition (rain, snow, thunderstorm, fog, etc.) ||
| 33 | Amenity | A POI annotation which indicates presence of [amenity](#) in a nearby location. | No |
| 34 | Bump | A POI annotation which indicates presence of [bump](#) in a nearby location. | No |
| 35 | Crossing | A POI annotation which indicates presence of [crossing](#) in a nearby location. | No |
| 36 | Give_Way | A POI annotation which indicates presence of [given_way](#) in a nearby location. | No |
| 37 | Junction | A POI annotation which indicates presence of [junction](#) in a nearby location. | No |
| 38 | No_Exit| A POI annotation which indicates presence of [no_exit](#) in a nearby location. | No |
| 39 | Railway | A POI annotation which indicates presence of [railway](#) in a nearby location. | No |
| 40 | Roundabout | A POI annotation which indicates presence of [roundabout](#) in a nearby location. | No |
| 41 | Station | A POI annotation which indicates presence of [station](#) in a nearby location. | No |
| 42 | Stop | A POI annotation which indicates presence of [stop](#) in a nearby location. | No |
| 43 | Traffic_Calming | A POI annotation which indicates presence of [traffic_calming](#) in a nearby location. | No |
| 44 | Traffic_Signal | A POI annotation which indicates presence of [traffic_signal](#) in a nearby location. | No |
| 45 | Turning_Loop | A POI annotation which indicates presence of [turning_loop](#) in a nearby location. | No |
| 46 | Sunrise_Sunset | Shows the daylight condition (day or night) based on sunrise/sunset. | Yes |
| 47 | Civil_Twilight | Shows the daylight condition (day or night) based on [civil twilight](#). | Yes |
| 48 | Nautical_Twilight | Shows the daylight condition (day or night) based on [nautical twilight](#). | Yes |
| 49 | Astronomical_Twilight | Shows the daylight condition (day or night) based on [astronomical twilight](#). | Yes |

## Applications of Dataset
US-Accidents can be used for numerous applications such as real-time accident prediction, studying accident hotspot locations, casualty analysis and extracting cause and effect rules to predict accidents, or studying the impact of precipitation or other environmental stimuli on accident occurrence. 
