---
layout: project-page
title: "Childhood Lead Poisoning in New York City"
linkname: childhood-lead-poisoning-in-new-york-city
author: "Kohinoor Begum"
tagline: "This interactive map features represent children under 6 year’s old age tested in NYC, 2016 year with blood lead levels of >=5 mcg/dL. My map will allow you to see what the local prevalence of elevated lead tests has been in NYC. It features interactive points and polygons that bring up corresponding details in the sidebar, options for zooming and showing, and a customized base map using Leaflet."
location:
    - place: New York City, New York, USA
project-link:
    - href: https://kohinoor-final-assignment-child-bloodlead.glitch.me/
tags:
    - tag: children, blood, lead level, NYC
thumbnail-path: img/childhood-lead-poisoning-in-new-york-city/imga.png
img-folder: ../../img/childhood-lead-poisoning-in-new-york-city/
timestamp: 3/24/2019 16:53:06
---

1\. My Project

Children are more vulnerable to lead poisoning in the first six years of life, particularly the first three, when the brain grows fastest, and when critical connections in the brain and nervous system control their learning, hearing, movement, behavior, and emotions are formed. Though New York City has dramatically reduced the number of children exposed to lead but hasn’t met its longstanding goal. Through my project, my goal was to create a map that allows users to compare the rate BLL >=5mg/dl (per 1000tested), 2016 across NYC.

2\. Why Map What I Mapped?

Lead is a toxic heavy metal that causes acute health impact. Today at least 4 million households have children living in them that are being exposed to high levels of lead. There are approximately half a million U.S. children ages 1-5 with blood lead levels above 5 micrograms per deciliter (µg/dL) Center For Disease Control and Prevention.

![]({{ page.img-folder }}img0.png)

Lead paint is the primary causes of childhood lead poisoning in NYC. Along with lead-based paint in old housing, the city’s children can face toxic hazards from consumer products, soil, and water. Recent research by the NYC Department of Health and Mental Hygiene shows that consumer products imported from South Asian Countries are contained a high level of lead. In addition to lead paint and occupational lead hazards, poisonings in this community have been associated with the use of traditional consumer products. As a result, New York City’s South Asian children and adults are especially at risk for lead poisoning.

![]({{ page.img-folder }}img1.png)

Figure: Metal Content of Consumer Products Tested by the NYC Health Department. A 2016 study found South Asian children in the city were six times more likely to have high blood lead levels than children citywide. Source: DOHMH ([NYC Open Data](https://data.cityofnewyork.us/Health/Metal-Content-of-Consumer-Products-Tested-by-the-N/da9u-wz3r/data).)

I am interested to do my research on human health exposure of lead hazard. To demonstrate my concern and become more familiar with this health issue, I choose this topic that will help me to spread my awareness against lead among the community. Here I used different color codes that will help you to easily understand the different rates of lead level toxicity in the five boroughs neighborhoods children.

3\.    Project Description

From my interest, I mapped NYC five boroughs based analysis of childhood under 6 years of age blood lead testing data at the neighborhood level. To map, I downloaded data from NYC Open Data source and cleaned up any unnecessary column and then filtered to keep only 2016 year dataset. The next step was to import the data into QGIS tool. In QGIS, I manipulated the data by following its many steps. Then I merged them with shapefile as my dataset did not contain any geometry. Then I uploaded the GeoJSON file in the Glitch site. After working some steps in Glitch, again I downloaded it from Glitch site to desktop and then drag it into the QGIS to change some of its features. With the help of QGIS, I made its column name shorter as the previous column name was too long to manage for pop up. Here I followed some complex but interesting steps to make column name shorter and change their data types from string to number to show them in pop up. Again, I uploaded the data in the QGIS and worked on it to make it final form.

To visualize the data, each neighborhood is represented by color according to their rate of the children BLL >=5 mcg/dl in that year 2016. The legend to indicate the rate is included on the bottom left corner of the map that represents their rate in descending order. When you will click anywhere on the map, a popup will show the name of the city, neighborhood, the number of tested children, elevated BLL rate per 1000 children.

4\.	Difficulties

Keeping track of javascript code.
Incorporate side bar in the map.
To remember and following step by step in QGIS to merging the data with shapefile as I don’t have prior experience in QGIS and mapping.
Javascript's different features and their sequences in the scrip still remains complex to understand.

5\.	Lesson Learned 

I learned lot of things from this course. But I think I need more practice as it is not easy to remember everything at a glance without practice.

6\. Next Steps

Add event listener with the help of D3. When hoving it will changes color for a second.
Find out census data to map census tract or zip code based map.

Find out the NYC South Asian communities neighborhoods data and incorporate them on the map to correlate their blood lead level and the consumer products having lead they consumed.

Zoom interactivity including "home zoom", conditional styling at different zoom levels.


7.    Data source <a href="https://data.cityofnewyork.us/Health/Children-Under-6-yrs-with-Elevated-Blood-Lead-Leve/tnry-kwh5/data" a> NYC Open Data</a>

* <a href ="https://kohinoor-final-assignment-spring-2019-savi-780.glitch.me/">Project Description on Glich</a>
* <a href ="https://kohinoor-final-assignment-child-bloodlead.glitch.me/">Link(s) to full project (Map)</a>
* <a href = "https://aurin77.github.io/child-lead/">Project on GitHub</a>
