---
title: "US-Accidents: A Countrywide Traffic Accident Dataset"
collection: datastes
permalink: /datasets/us_accidents
excerpt: This is a countrywide motor-vehicle crash dataset, which covers 49 states of the United States. The data is continuously being collected from February 2016. Currently, there are 2.25 million accident records in this dataset. Each accident record is described by a variety of attributes including location, time, weather, and nearby points-of-intertest. 
date: 2019-05-05
---

## Description 
This is a countrywide traffic accident dataset, which covers 49 states of the United States. The data is continuously being collected from February 2016, using several data providers, including two APIs which provide streaming traffic event data. These APIs broadcast traffic events captured by a variety of entities, such as the US and state departments of transportation, law enforcement agencies, traffic cameras, and traffic sensors within the road-networks. Currently, there are about 2.25 million accident records in this dataset. Check the below descriptions for more detailed information. 

## Acknowledgment
Please cite the following paper if you use this dataset:

* Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, and Rajiv Ramnath. ["A Countrywide Traffic Accident Dataset."](#), 2019. 

## Usage Policy and Legal Disclaimer
This dataset is being distributed only for __Research__ purposes, under [Creative Commons Attribution-Noncommercial-ShareAlike license (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/){:target="_blank"}. By clicking on download button(s) below, you are agreeing to use this data only for non-commercial, research, or academic applications. 


## Download
* __Version 1 (May 2019):__ In this version, we provide data which is collected from February 2016 to March 2019 for the [Contiguous United States](https://en.wikipedia.org/wiki/Contiguous_United_States){:target="_blank"}. In this set, we have about 2.25 million traffic accidents. Download data from [here](https://osu.app.box.com/v/us-accidents){:target="_blank"}. 

The next version will be available by October 2019. 


## Coverage
The dataset covers 49 US States. Following diagram shows the current data distribution over all the states. 

## Format
The data is provided in terms of a __single CSV file__. Following table describes the data attributes: 

| \# | Attribute | Description | Nullable |
|:------:|:---------:|-------------|:--------:|
| 1 | ID | This is the unique identifier of the accident record. | No |
| 2 | Source | Indicates the source of the accident report (i.e. the API which reported the accident.). | No |
| 3 | TMC | A traffic accident may have a [Traffic Message Channel (TMC)](https://wiki.openstreetmap.org/wiki/TMC/Event_Code_List){:target="_blank"} code which provides more detailed description of the event. | Yes |
| 4 | Severity | Shows the severity of the accident (a number between 1 and 4). | No |
| 5 | Start_Time | Shows the start time of the accident in local time zone. | No |
| 6 | End_Time | Shows the end time of the accident in local time zone. | No |
| 7 | Start_Lat | Shows the latitude in GPS coordinate of start point. | No |
| 8 | Start_Lng | Shows the longitude in GPS coordinate of start point. | No |
| 9 | End_Lat | Shows the latitude in GPS coordinate of end point. | Yes |
| 10 | End_Lng | Shows the longitude in GPS coordinate of end point. | Yes |
| 11 | Distance(mi) | The length of the road extent affected by the accident. | No |
| 12 | Description | Shows the natural language description of the accident. | No |
| 13 | Number | Shows the street number in address field. | Yes |
| 14 | Street | Shows the street name in address field.  | Yes |
| 15 | Side | Shows the relative side of the street (Right/Left) in address field. | Yes |
| 16 | City | Shows the city in address field. | Yes |
| 17 | County | Shows the county in address field. | Yes |
| 18 | State | Shows the state in address field. | Yes |
| 19 | Zipcode | Shows the zipcode in address field. | Yes |
| 20 | Country | Shows the country in address field. | Yes |
| 21 | Timezone | Shows the timezone based on the location of an accident (eastern, central, etc.). | Yes |
| 22 | Airport_Code | Denotes the airport-based weather station which is the closest one to the location of the accident. | Yes |
| 23 | Weather_Timestamp | Shows the time-stamp of weather observation record in local time. | Yes |
| 24 | Temperature(F) | Shows the temperature in Fahrenheit. | Yes |
| 25 | Wind_Chill(F) | Shows the wind chill in Fahrenheit. | Yes |
| 26 | Humidity(%) | Shows the humidity in percentage. | Yes |
| 27 | Pressure(in) | Shows the air pressure in inches. | Yes |
| 28 | Visibility(mi) | Shows visibility in miles. | Yes |
| 29 | Wind_Direction | Shows wind direction. | Yes |
| 30 | Wind_Speed(mph) | Shows wind speed in miles per hour. | Yes |
| 31 | Precipitation(in) | Shows precipitation amount in inches, if there is any. | Yes |
| 32 | Weather_Condition | Shows the weather condition (rain, snow, thunderstorm, fog, etc.) | Yes |
| 33 | Amenity | A POI annotation which indicates presence of [amenity](https://wiki.openstreetmap.org/wiki/Key:amenity) in a nearby location. | No |
| 34 | Bump | A POI annotation which indicates presence of speed bump or hump in a nearby location. | No |
| 35 | Crossing | A POI annotation which indicates presence of [crossing](https://wiki.openstreetmap.org/wiki/Key:crossing) in a nearby location. | No |
| 36 | Give_Way | A POI annotation which indicates presence of [give_way](https://wiki.openstreetmap.org/wiki/Tag:highway%3Dgive_way) in a nearby location. | No |
| 37 | Junction | A POI annotation which indicates presence of [junction](https://wiki.openstreetmap.org/wiki/Key:junction) in a nearby location. | No |
| 38 | No_Exit| A POI annotation which indicates presence of [no_exit](https://wiki.openstreetmap.org/wiki/Key:noexit) in a nearby location. | No |
| 39 | Railway | A POI annotation which indicates presence of [railway](https://wiki.openstreetmap.org/wiki/Key:railway) in a nearby location. | No |
| 40 | Roundabout | A POI annotation which indicates presence of [roundabout](https://wiki.openstreetmap.org/wiki/Tag:junction%3Droundabout) in a nearby location. | No |
| 41 | Station | A POI annotation which indicates presence of [station](https://wiki.openstreetmap.org/wiki/Key:station) in a nearby location. | No |
| 42 | Stop | A POI annotation which indicates presence of [stop](https://wiki.openstreetmap.org/wiki/Key:stop) in a nearby location. | No |
| 43 | Traffic_Calming | A POI annotation which indicates presence of [traffic_calming](https://wiki.openstreetmap.org/wiki/Key:traffic_calming) in a nearby location. | No |
| 44 | Traffic_Signal | A POI annotation which indicates presence of [traffic_signal](https://wiki.openstreetmap.org/wiki/Tag:highway%3Dtraffic_signals) in a nearby location. | No |
| 45 | Turning_Loop | A POI annotation which indicates presence of [turning_loop](https://wiki.openstreetmap.org/wiki/Tag:highway%3Dturning_loop) in a nearby location. | No |
| 46 | Sunrise_Sunset | Shows the period of day (day or night) based on sunrise/sunset. | Yes |
| 47 | Civil_Twilight | Shows the period of day (day or night) based on [civil twilight](https://en.wikipedia.org/wiki/Twilight#Civil_twilight). | Yes |
| 48 | Nautical_Twilight | Shows the period of day (day or night) based on [nautical twilight](https://en.wikipedia.org/wiki/Twilight#Nautical_twilight). | Yes |
| 49 | Astronomical_Twilight | Shows the period of day (day or night) based on [astronomical twilight](https://en.wikipedia.org/wiki/Twilight#Astronomical_twilight). | Yes |

## Applications of Dataset
US-Accidents can be used for numerous applications such as real-time accident prediction, studying accident hotspot locations, casualty analysis and extracting cause and effect rules to predict accidents, or studying the impact of precipitation or other environmental stimuli on accident occurrence. 
