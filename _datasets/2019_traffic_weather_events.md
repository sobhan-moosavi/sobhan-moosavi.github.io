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
The data coverage is country-wide. It currently contains data for the [Contiguous United States](https://en.wikipedia.org/wiki/Contiguous_United_States){:target="_blank"}. Following diagrams show the number of data records (i.e., events) based on traffic or weather for different states. 

<div class="mxgraph" style="max-width:100%;border:1px solid transparent;" data-mxgraph="{&quot;highlight&quot;:&quot;#0000ff&quot;,&quot;nav&quot;:true,&quot;resize&quot;:true,&quot;toolbar&quot;:&quot;zoom layers lightbox&quot;,&quot;edit&quot;:&quot;_blank&quot;,&quot;xml&quot;:&quot;&lt;mxfile modified=\&quot;2019-02-03T01:39:12.872Z\&quot; host=\&quot;www.draw.io\&quot; agent=\&quot;Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/71.0.3578.98 Safari/537.36\&quot; etag=\&quot;9bPxho-f9Ks2Qngdc51X\&quot; version=\&quot;10.1.6-6\&quot; type=\&quot;device\&quot;&gt;&lt;diagram id=\&quot;c562b6ec-9891-0046-892f-c501f7719b2d\&quot; name=\&quot;Page-1\&quot;&gt;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&lt;/diagram&gt;&lt;/mxfile&gt;&quot;}"></div>

<script type="text/javascript" src="https://www.draw.io/js/viewer.min.js"></script>

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
This dataset is being distributed only for __Research__ purposes, under [Creative Commons Attribution-Noncommercial-ShareAlike license (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/){:target="_blank"}. By clicking on download button(s) below, you may accept that you will use this data only for non-commercial, research, or academic applications. 

## Download
* __Version 1 (Aug 2018):__ In this version, we provide data which is collected from August 2016 to August 2018 for the Contiguous United States. In this set, we have about 13.1 million traffic and 2.2 million weather event records. Download data from [here](#). 

<!--- __Download Version 2 (Dec 2018):__ In this version, we provide data which is collected from August 2016 to December 2018 for the Contiguous United States. In this set, we have ?? million traffic and ?? million weather event records. Download from [here](#). -->

## Applications of Dataset

## Acknowledgments
