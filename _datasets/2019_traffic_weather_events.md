---
title: "Large-Scale Traffic and Weather Entity Dataset"
collection: datastes
permalink: /datasets/2019_traffic_weather_events
excerpt: This dataset contains country-wide traffic or weather entities, which are continuously being collected from August 2016. Examples of a traffic entity are *accident*, *congestion*, and *construction*. Examples of a weather entity are *rain*, *snow*, and *storm*. 
date: 2019-01-01
---
## Description 
This dataset is a large-scale, unique source of data for transportation and traffic research, which contains traffic and weather entities. In terms of traffic, we have several types of traffic entity including accident, congestion, construction, etc. In terms of weather entities, we have several types including rain, snow, storm, cold weather, etc. This dataset has been collected from August 2016, and is continuously being updated. 

## Traffic Entity
Traffic entity is a spatiotemporal entity, where such entity is associated with location and time. Following table describes different types of traffic entity in our dataset: 

| Type | Description |
|------|-------------|
| Accident | A traffic accidnet which can involve one or more vehicles. |
| Broken-Vehicle | Refers to the situation when there is one (or more) disabled vehicle(s) in a road. |
| Congestion | Refers to the situation when the speed of traffic is lower than the expected speed. |
| Construction | Refers to an on-going construction or re-paring project in a road. |
| Event | Refers to the situations such as *sport event*, *concert*, and *demonstration*. |
| Lane-Blocked | Refers to the cases when we have blocked lane(s) due to traffic or weather condition. |
| Flow-Incident | Refers to all other types of traffic entities. Examples are *broken traffic light* and *animal in the road*. |

## Weather Entity
Weather entity is a spatiotemporal entity, where such entity is associated with location and time. Following table describes different types of weather entity in our dataset: 

| Type | Description |
|------|-------------|
| Severe-Cold | The case of having extremely low temperature, with ```temperature < -23.7``` degree of celsius. |
| Fog | The case where there is low visibility condition as result of *fog* or *haze*. |
| Hail | The case of having solid precipitation including *ice pallets* and *hail*. |
| Rain | The case of having rain, including any type of the rain, ranging from *light* to *heavy*. |
| Snow | The case of having snow, including any type, ranging from *light* to *heavy*. |
| Storm | The extremely windy condition, where the wind speed is at least *60 kmh*. |
| Other Precipitation | any other type of of precipitation which cannot be assigned to previously described entity types. |

## Collection Process

## Coverage
The data coverage is country-wide. It currently contains data for the [Contiguous United States](https://en.wikipedia.org/wiki/Contiguous_United_States){:target="_blank"}. Following diagrams show the number of data records (i.e., events) based on traffic or weather for different states. 

## Format and Download

## Applications of Dataset

## Acknowledgments
