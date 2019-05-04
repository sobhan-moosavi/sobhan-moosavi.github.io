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

* Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, and Rajiv Ramnath. ["US-Accidents: A Countrywide Traffic Accident Dataset."](#), 2019. 

## Usage Policy and Legal Disclaimer
This dataset is being distributed only for __Research__ purposes, under [Creative Commons Attribution-Noncommercial-ShareAlike license (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/){:target="_blank"}. By clicking on download button(s) below, you are agreeing to use this data only for non-commercial, research, or academic applications. 


## Download
* __Version 1 (May 2019):__ In this version, we provide data which is collected from February 2016 to March 2019 for the [Contiguous United States](https://en.wikipedia.org/wiki/Contiguous_United_States){:target="_blank"}. In this set, we have about 2.25 million traffic accidents. Download data from [here](#){:target="_blank"}. 


## Format
The data is provided in terms of a __single CSV file__. Following table describes the data attributes: 

| Number | Attribute | Description | Nullable |
|:------:|:---------:|-------------|:--------:|
| 1 | ID | This is the unique identifier of an accident record | No |
| 2 | Source | Indicates the source of an event which can be MapQuest, Bing, or both. | No |
| 3 | TMC | A traffic accident may have a [Traffic Message Channel (TMC)](https://wiki.openstreetmap.org/wiki/TMC/Event_Code_List){:target="_blank"} code which provides more detailed description of the event. | Yes |
| 4 | Severity | Shows the severity of an event, wherever applicable. | Yes |
| 5 | StartTime | Shows the start time of an event in UTC time zone. | No |
| | EndTime | Shows the end time of an event in UTC time zone. | No |
| | Start_Lat | Shows the latitude in GPS coordinate for start point. | Yes |
| | Start_Lng | Shows the longitude in GPS coordinate for start point. | Yes |
| | End_Lat | Shows the latitude in GPS coordinate for end point. | Yes |
| | End_Lng | Shows the longitude in GPS coordinate for end point. | Yes |
| | Distance (mi) | Shows the radius of impact. | Yes |
| | Description | Shows the natural language description of the accident. | Yes |
| | Number | Shows the street number in address field. | Yes |
| | Street | Shows the street name in address field.  | Yes |
| | Side | Shows the relative side of a street (R/L) in address field. | Yes |
| | City | Shows the city in address field. | Yes |
| | County | Shows the county in address field. | Yes |
| | State | Shows the state in address field. | Yes |
| | ZipCode | Shows the zipcode in address field. | Yes |
| | Timezone | Shows the timezone based on the location of an accident. | Yes |
| | AirportCode | Shows the closest weather station to the reported accident. | Yes |
| | Timestamp |||
| | Temperature (F) |||
| | Wind_Chill (F) |||
| | Humidity (%) |||
| | Pressure () |||
| | Visibility (mi) |||
| | Wind_Direction |||
| | Wind_Speed (mph) |||
| | Precipitation () |||
| | Condition |||
| | Amenity |||
| | Bump |||
| | Crossing |||
| | Give_Way |||
| | Junction |||
| | No_Exit|||
| | Railway |||
| | Roundabout |||
| | Station |||
| | Stop |||
| | Traffic_Calming |||
| | Traffic_Signal |||
| | Turning_Loop |||
| | Sunrise_Sunset |||
| | Civil_Twilight |||
| | Nautical_Twilight |||
| | Astronomical_Twilight |||


## Coverage
The data coverage is country-wide. Following diagram shows the current data distribution over all the states. 

## Applications of Dataset
US-Accidents can be used for numerous applications such as real-time accident prediction, studying accident hotspot locations, casualty analysis and extracting cause and effect rules to predict accidents, or studying the impact of precipitation or other environmental stimuli on accident occurrence. 
