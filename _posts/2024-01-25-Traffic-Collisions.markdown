---
layout: post
title: Traffic Collisions 2017-2021
description:
img: /TrafficAccidentMap/Preview.png
fig-caption:
tags:
carousels:
  - images:
    - image: /assets/img/TrafficAccidentMap/2017.png
    - image: /assets/img/TrafficAccidentMap/2018.png
    - image: /assets/img/TrafficAccidentMap/2019.png
    - image: /assets/img/TrafficAccidentMap/2020.png
    - image: /assets/img/TrafficAccidentMap/2021.png
---

*This is an independent project worked on during my time in school. Although the data indeed shows a correlation over time of an increase in reported accidents by police departments, the results of this work also created more questions between myself and my teacher as to the reasons why.*

# Frequency of accidents in San Diego County from 2015 - 2022

## *Problem Statement*
Personal experience when driving on the roads of San Diego after the Covid pandemic has led me to believe people are much less attentive when driving their vehicles. This project will be utilizing San Diego Police Department reports to determine an increase, decrease, or no change in the rate of traffic accidents over a 5-year period (2016 – 2021).

## *Data inconsistencies & errors*
Vehicle Accidents reported from San Diego Police Department does not include highways or freeways.

From the DataSD website for the Traffic Collision reports: “Generally a report is not taken for property damage-only collisions that do not involve hit & run or DUI.” This does not exclude all incidents where hit & run or DUI does not occur, however it does exclude other incidents, which makes this data not complete when looking at total number of actual vehicle accidents that occur.

There are a total of 118,468 points for the years 2015-2022; When geocoding for the map, only 106,763 data points were matched accurately. This difference of 11,705, or 9.88%, are unmatched or tied and not included

Final numbers in this report are pulled from the .csv obtained from Data SD. See figure 1 for information regarding missing entries.

## *Accidents per year*
Total numbers have been calculated from the data provided by DataSD Traffic Collisions report. Figure 1 shows the number of matched, geocoded locations from the provided data, along with the number of locations that failed to match. These numbers matter for the heatmaps further in this report.

***Figure 1:***

|   |   |   |   |   |
|---|---|---|---|---|
|**Year**|**Total Accidents**|**_Matched on map_**|**_Unmatched_**|**_% Error_**|
|2017|15,542|15,486|56|0.36 %|
|2018|15,034|14,992|42|0.28 %|
|2019|18,120|17,997|123|0.68 %|
|2020|17,072|16,897|175|1.02 %|
|2021|19,706|19,530|176|0.89 %|

## *Rate of change year over year*
Rate of accident increases, or decreases, are shown in Figure 2. The year 2016, which had 16,021 reported accidents, has been included for calculating 2017 rate of change.

***Figure 2:***

|   |   |   |   |
|---|---|---|---|
|**Year**|**Total Accidents**|**Change from previous year**|**% of change**|
|2017|15,542|- 479|- 2.99 %|
|2018|15,034|- 508|- 3.27 %|
|2019|18,120|+ 3,086|+ 20.53 %|
|2020|17,072|- 1,048|- 5.78 %|
|2021|19,706|+ 2,634|+ 15.43 %|

## *Vehicle accident heatmaps*
The following pages show heatmaps of accidents per year from 2017–2021. Points considered are within a 1.25mi radius.

{% include carousel.html height=auto unit="%" duration="10" number="1" %}

<!--
![2017]({{site.baseurl}}/assets/img/TrafficAccidentMap/2017.png)
![2018]({{site.baseurl}}/assets/img/TrafficAccidentMap/2018.png)
![2019]({{site.baseurl}}/assets/img/TrafficAccidentMap/2019.png)
![2020]({{site.baseurl}}/assets/img/TrafficAccidentMap/2020.png)
![2021]({{site.baseurl}}/assets/img/TrafficAccidentMap/2021.png)
-->

## *Conclusion*
The data pulled from the Traffic Collisions report clearly shows an overall increase in traffic accidents on the roads of San Diego over the past 5 years. From 2015 to 2021, there was an average increase of 737 accidents per year, with an increase of over 4,000 reported accidents in 2021 compared with 2015. Population or driver increases, or decreases, have not been considered. This report only shows a flat increase or decrease in number of accidents involving a police report, which is still a significant number. Police reports would be expected to maintain a standard for when a vehicle accident would be reported, so this information should remain relatively consistent year over year.

## *Sources*
SANDAG. “Roads All.” SANDAG/SanGIS Regional GIS Data Warehouse Open Data Portal, SANDAG, 7 Sept. 2018, [https://sdgis-sandag.opendata.arcgis.com/datasets/SANDAG::roads-all/about](https://sdgis-sandag.opendata.arcgis.com/datasets/SANDAG::roads-all/about).

SANDAG. “Census Tracts.” SANDAG/SanGIS Regional GIS Data Warehouse Open Data Portal, SANDAG, 9 July 2018, [https://sdgis-sandag.opendata.arcgis.com/datasets/census-tracts/explore?location=33.039400%2C-116.844950%2C9.65](https://sdgis-sandag.opendata.arcgis.com/datasets/census-tracts/explore?location=33.039400%2C-116.844950%2C9.65).

City of San Diego. “Traffic Collisions - People and Vehicles Involved - City of San Diego Open Data Portal.” _City of San Diego Open Data Portal_, San Diego Police Department, 22 Mar. 2022, [https://data.sandiego.gov/datasets/police-collisions-details/](https://data.sandiego.gov/datasets/police-collisions-details/).
