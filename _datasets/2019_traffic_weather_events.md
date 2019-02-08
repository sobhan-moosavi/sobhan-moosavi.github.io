---
title: "Large-Scale Traffic and Weather Events Dataset"
collection: datastes
permalink: /datasets/2019_traffic_weather_events
excerpt: This dataset contains country-wide traffic or weather events, which are continuously being collected from August 2016. Examples of a traffic event are *accident*, *congestion*, and *construction*. Examples of a weather event are *rain*, *snow*, and *storm*. 
date: 2019-02-03
---
## Description 
This dataset is a large-scale, unique source of data for transportation and traffic research, which contains traffic and weather events. In terms of traffic, we have several types of traffic event including accident, congestion, construction, etc. In terms of weather events, we have several types including rain, snow, storm, cold weather, etc. This dataset has been collected from August 2016, and is continuously being updated. For more detailed information about this dataset, please read [this paper](#){:target="_blank"}. 

## Traffic Events
Traffic event is a spatiotemporal entity, where such entity is associated with location and time. Following table describes different types of traffic event in our dataset. Note that for several of event types such as congestion and construction, we also included severity of the event in the *type* attribute. <!---For construction and event, severity is determined based on duration. For congestion, severity is determined by speed of the congestion. -->

| Type | Description | Severity |
|------|-------------|----------|
| Accident | A traffic accident which can involve one or more vehicles. | N/A |
| Broken-Vehicle | Refers to the situation when there is one (or more) disabled vehicle(s) in a road. | N/A |
| Congestion | Refers to the situation when the speed of traffic is lower than the expected speed. | Slow, Moderate, Fast |
| Construction | Refers to an on-going construction or re-paring project in a road. | Short, Long |
| Event | Refers to the situations such as *sport event*, *concert*, and *demonstration*. | Short, Long|
| Lane-Blocked | Refers to the cases when we have blocked lane(s) due to traffic or weather condition. | N/A |
| Flow-Incident | Refers to all other types of traffic entities. Examples are *broken traffic light* and *animal in the road*. | |

## Weather Events
Weather event is a spatiotemporal entity, where such entity is associated with location and time. Following table describes different types of weather events in our dataset. We also provided severity of rain and snow in our dataset. To do so, we used observation of precipitation amount for each case for a long period of time, performed k-means clustering, and for each case identified three clusters in terms of *light*, *moderate*, and *heavy*. More details can be find [here](#){:target="_blank"}.

| Type | Description | Severity |
|------|-------------|----------|
| Severe-Cold | The case of having extremely low temperature, with temperature below *-23.7* degrees of Celsius. | Severe |
| Fog | The case where there is low visibility condition as result of *fog* or *haze*. |  |
| Hail | The case of having solid precipitation including *ice pallets* and *hail*. | N/A |
| Rain | The case of having rain. | Light, Moderate, and Heavy |
| Snow | The case of having snow. | Light, Moderate, and Heavy |
| Storm | The extremely windy condition, where the wind speed is at least *60 kmh*. | Severe |
| Other Precipitation | Any other type of of precipitation which cannot be assigned to previously described entity types. |  |

## Collection Process
Traffic data is collected from [MapQuest](https://www.mapquest.com/) using an API, for a period of two years. Weather data is collected from [Weather Underground](https://www.wunderground.com/) using their API for the same period of time (i.e., from August 2016 to August 2018). Plesse visit [our paper](#) to learn more about the data collection and processing steps. 


## Coverage
The data coverage is country-wide. It currently contains data for the [Contiguous United States](https://en.wikipedia.org/wiki/Contiguous_United_States){:target="_blank"}. Following diagram shows the frequency distribution of traffic events across 50 difference states in US. 

<iframe frameborder="0" scrolling="no" src="//plot.ly/~sobhan.mehr84/8.embed" style="height: 100%; width: 500;"></iframe>

The next diagram shows the frequency distribution of weather events for the same set of staes. 

<iframe frameborder="0" scrolling="no" src="//plot.ly/~sobhan.mehr84/6.embed" style="height: 100%; width: 500;"></iframe>



## Format
The data is provided in the format of CSV files. Following table describes the data attributes: 

| Attribute | Description | Nullable |
|:---------:|-------------|:--------:|
| ID | This is the identifier of a record | No |
| Type (T/W) | Indicates whether the entity is a traffic (T) or weather (W) event. | No |
| RefinedType | Shows the type of the event, examples are *rain*, *snow*, *accident*, etc. | No |
| Severity | Shows the severity of an event, wherever applicable. | Yes |
| StartTime (UTC) | Shows the start time of the event in UTC time zone. | No |
| EndTime (UTC) | Shows the end time of the event in UTC time zone. | No |
| LocationLat | Shows the latitude of GPS coordinate. | Yes |
| LocationLng | Shows the longitude of GPS coordinate. | Yes |
| Distance (mi) | Shows the radius of impact by a traffic event. | Yes |
| AirportCode | Shows the airport station that a weather event is reported from. | Yes |
| Number | Shows the street number in address field. | Yes |
| Street | Shows the street name in address field.  | Yes |
| Side | Shows the relative side of a street (R/L) in address field. | Yes |
| City | Shows the city in address field. | Yes |
| County | Shows the county in address field. | Yes |
| State | Shows the State in address field. | Yes |
| ZipCode | Shows the zipcode in address field. | Yes |

## Usage Policy and Legal Disclaimer
This dataset is being distributed only for __Research__ purposes, under [Creative Commons Attribution-Noncommercial-ShareAlike license (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/){:target="_blank"}. By clicking on download button(s) below, you are agreeing to use this data only for non-commercial, research, or academic applications. 

## Download
* __Version 1 (Aug 2018):__ In this version, we provide data which is collected from August 2016 to August 2018 for the Contiguous United States. In this set, we have about 13.1 million traffic and 2.2 million weather event records. Download data from [here](#). 

<!--- __Download Version 2 (Dec 2018):__ In this version, we provide data which is collected from August 2016 to December 2018 for the Contiguous United States. In this set, we have ?? million traffic and ?? million weather event records. Download from [here](#). -->

## Applications of Dataset

## Acknowledgments
