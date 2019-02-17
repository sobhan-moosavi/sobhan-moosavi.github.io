---
title: "Large-Scale Traffic and Weather Events Dataset"
collection: datastes
permalink: /datasets/2019_traffic_weather_events
excerpt: This dataset contains country-wide traffic or weather events, which are continuously being collected from August 2016. Examples of a traffic event are *accident*, *congestion*, and *construction*. Examples of a weather event are *rain*, *snow*, and *storm*. 
date: 2019-02-03
---
## Description 
This dataset is a large-scale, unique source of data for transportation and traffic research, which contains traffic and weather events. In terms of traffic, we have several types of traffic event including accident, congestion, construction, etc. In terms of weather events, we have several types including rain, snow, storm, cold weather event, etc. This dataset is being continuously collected from August 2016. For more detailed information about this dataset, please read below descriptions. 


## Acknowledgment
Please cite the following paper if you use this dataset:

* Sobhan Moosavi, Mohammad Hossein Samavatian, Arnab Nandi, Srinivasan Parthasarathy and Rajiv Ramnath; ["Short and Long-term Pattern Discovery Over Large-Scale Geo-Spatiotemporal Data"](#){:target="_blank"}, 2019


## Usage Policy and Legal Disclaimer
This dataset is being distributed only for __Research__ purposes, under [Creative Commons Attribution-Noncommercial-ShareAlike license (CC BY-NC-SA 4.0)](https://creativecommons.org/licenses/by-nc-sa/4.0/){:target="_blank"}. By clicking on download button(s) below, you are agreeing to use this data only for non-commercial, research, or academic applications. 


## Download
* __Version 1 (Aug 2018):__ In this version, we provide data which is collected from August 2016 to August 2018 for the [Contiguous United States](https://en.wikipedia.org/wiki/Contiguous_United_States){:target="_blank"}. In this set, we have about 13.2 million traffic and 2.3 million weather event records. Download data from [here](https://osu.box.com/s/ggsyjum4km33g25yfvihcx2mfkj2mu69){:target="_blank"}. 

<!--- __Download Version 2 (Dec 2018):__ In this version, we provide data which is collected from August 2016 to December 2018 for the Contiguous United States. In this set, we have ?? million traffic and ?? million weather event records. Download from [here](#). -->


## Format
The data is provided in terms of CSV files. Following table describes the data attributes: 

| Attribute | Description | Nullable |
|:---------:|-------------|:--------:|
| ID | This is the identifier of a record | No |
| Source | Indicates the source of an event which is either traffic (T) or weather (W). | No |
| Type | Shows the type of an event; examples are *rain*, *snow*, *accident*, etc. | No |
| TMC | Each traffic event has a [Traffic Message Channel (TMC)](https://wiki.openstreetmap.org/wiki/TMC/Event_Code_List){:target="_blank"} code which defines its type. | Yes |
| Severity | Shows the severity of an event, wherever applicable. | Yes |
| StartTime (UTC) | Shows the start time of an event in UTC time zone. | No |
| EndTime (UTC) | Shows the end time of an event in UTC time zone. | No |
| LocationLat | Shows the latitude in GPS coordinate. | Yes |
| LocationLng | Shows the longitude in GPS coordinate. | Yes |
| Distance (mi) | Shows the radius of impact by a traffic event. | Yes |
| AirportCode | Shows the airport station that a weather event is reported from, or the closest airport station to the location of a traffic event. | Yes |
| Number | Shows the street number in address field of a traffic event. | Yes |
| Street | Shows the street name in address field of a traffic event.  | Yes |
| Side | Shows the relative side of a street (R/L) in address field of a traffic event. | Yes |
| City | Shows the city in address field. | Yes |
| County | Shows the county in address field of a traffic event. | Yes |
| State | Shows the State in address field. | Yes |
| ZipCode | Shows the zipcode in address field of a traffic event. | Yes |


## Traffic Events
Traffic event is a spatiotemporal entity, where such entity is associated with location and time. Following table describes different types of traffic event in our dataset. Visit [our paper](#){:target="_blank"} to learn how we determine severity of traffic events.

| Type | Description | Severity |
|------|-------------|----------|
| Accident | A traffic accident which can involve one or more vehicles. | N/A |
| Broken-Vehicle | Refers to the situation when there is one (or more) disabled vehicle(s) in a road. | N/A |
| Congestion | Refers to the situation when the speed of traffic is lower than the expected speed. | Slow, Moderate, Fast |
| Construction | Refers to an on-going construction or re-paring project in a road. | Short, Long |
| Event | Refers to the situations such as *sport event*, *concert*, and *demonstration*. | Short, Long|
| Lane-Blocked | Refers to the cases when we have blocked lane(s) due to traffic or weather condition. | N/A |
| Flow-Incident | Refers to all other types of traffic events. Examples are *broken traffic light* and *animal in the road*. | N/A |


## Weather Events
Weather event is a spatiotemporal entity, where such entity is associated with location and time. Following table describes different types of weather events in our dataset. Visit [our paper](#){:target="_blank"} to learn how we determine severity of weather events. 

| Type | Description | Severity |
|------|-------------|----------|
| Severe-Cold | The case of having extremely low temperature, with temperature below *-23.7* degrees of Celsius. | Severe |
| Fog | The case where there is low visibility condition as result of *fog* or *haze*. | N/A |
| Hail | The case of having solid precipitation including *ice pallets* and *hail*. | N/A |
| Rain | The case of having rain. | Light, Moderate, and Heavy |
| Snow | The case of having snow. | Light, Moderate, and Heavy |
| Storm | The extremely windy condition, where the wind speed is at least *60 kmh*. | Severe |
| Other Precipitation | Any other type of of precipitation which cannot be assigned to previously described event types. | N/A |


## Collection Process
Raw traffic data is collected in __real-time__ using an API from [MapQuest](https://www.mapquest.com/), for a period of two years. Raw weather data is collected using an API from [Weather Underground](https://www.wunderground.com/){:target="_blank"} for the same period of time (i.e., from August 2016 to August 2018). Please visit [our paper](#){:target="_blank"} to learn more about the data collection and processing steps. 


## Coverage
The data coverage is country-wide. It currently contains data for the [Contiguous United States](https://en.wikipedia.org/wiki/Contiguous_United_States){:target="_blank"}. Following diagram shows the current frequency distribution of __traffic__ events across 50 difference states in US. 

__Note__: For the following states, we have no traffic data from August 2016 to August 2017: AL, AR, AZ, CO, ID, KS, KY, LA, ME, MN, MS, MT, NC, ND, NH, NM, NV, OK, OR, SD, TN, UT, VT, WI, and WY. 

<div>
    <a href="https://plot.ly/~sobhan.mehr84/19/?share_key=Ca02M65nSgHpcvhv9Nh1Pm" target="_blank" title="traffic_frequency" style="display: block; text-align: center;"><img src="https://plot.ly/~sobhan.mehr84/19.png?share_key=Ca02M65nSgHpcvhv9Nh1Pm" alt="traffic_frequency" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="sobhan.mehr84:19" sharekey-plotly="Ca02M65nSgHpcvhv9Nh1Pm" src="https://plot.ly/embed.js" async></script>
</div>


The next diagram shows the current frequency distribution of __weather__ events for the same set of states. 

<div>
    <a href="https://plot.ly/~sobhan.mehr84/6/?share_key=aRlIZieZPkcZSt4QZEHzG7" target="_blank" title="weather_frequency" style="display: block; text-align: center;"><img src="https://plot.ly/~sobhan.mehr84/6.png?share_key=aRlIZieZPkcZSt4QZEHzG7" alt="weather_frequency" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="sobhan.mehr84:6" sharekey-plotly="aRlIZieZPkcZSt4QZEHzG7" src="https://plot.ly/embed.js" async></script>
</div>

Following diagram shows the current distribution of different __traffic__ event types: 

<div>
    <a href="https://plot.ly/~sobhan.mehr84/12/?share_key=RYBxrTEZBjbkqrjKQ8pM9F" target="_blank" title="traffic_types" style="display: block; text-align: center;"><img src="https://plot.ly/~sobhan.mehr84/12.png?share_key=RYBxrTEZBjbkqrjKQ8pM9F" alt="traffic_types" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="sobhan.mehr84:12" sharekey-plotly="RYBxrTEZBjbkqrjKQ8pM9F" src="https://plot.ly/embed.js" async></script>
</div>


Similarly, current distribution of __weather__ event types is shown in below diagram: 

<div>
    <a href="https://plot.ly/~sobhan.mehr84/17/?share_key=MkdsnbKws2tHQVyaZvjVU7" target="_blank" title="weather_types" style="display: block; text-align: center;"><img src="https://plot.ly/~sobhan.mehr84/17.png?share_key=MkdsnbKws2tHQVyaZvjVU7" alt="weather_types" style="max-width: 100%;width: 600px;"  width="600" onerror="this.onerror=null;this.src='https://plot.ly/404.png';" /></a>
    <script data-plotly="sobhan.mehr84:17" sharekey-plotly="MkdsnbKws2tHQVyaZvjVU7" src="https://plot.ly/embed.js" async></script>
</div>


## Applications of Dataset
This dataset can be used for plenty of purposes such as traffic analysis and prediction, impact prediction, accident prediction,  routing engine optimization, travel time estimation, and many other research applications. 


### 
__Page Visits:__  <a href='https://www.stat-counter.org/'>Counter Widget</a> <script type='text/javascript' src='https://www.freevisitorcounters.com/auth.php?id=cb0c83df897583dfb6d8272b30d1adf869fb7ecd'></script> <script type="text/javascript" src="https://www.freevisitorcounters.com/en/home/counter/487718/t/5"></script>
