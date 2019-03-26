---
layout: project-page
title: "Boba vs. Bubble Tea"
linkname: boba-vs-bubble-tea
author: "Jess Bagtas"
tagline: "Based on an online survey conducted by the Asian Americana podcast in 2017, this map shows the regional differences in what people call this popular Asian drink: Bubble tea or Boba?"
location:
    - place: USA
project-link:
    - href: https://bagtas3.github.io/BobaProject/examples/html/bobamap.html
tags:
    - tag: bubble tea
    - tag:  boba
    - tag: food
    - tag: culture
    - tag: cultural differences
    - tag: linguistics
    - tag:  regional differences
    - tag: regional variations
    - tag: drinks
    - tag: asian cuisine
    - tag: cuisine
    - tag: asia
    - tag: asian american
    - tag: asian america
thumbnail-path: img/boba-vs-bubble-tea/2QgPlX6.png
img-folder: ../../img/boba-vs-bubble-tea/
timestamp: 3/25/2019 9:21:51
---
Background:

According to Wikipedia, bubble tea or boba is  “a Taiwanese tea-based drink invented in Tainan and Taichung in the 1980s. Recipes contain tea of some kind, flavors of milk, as well as sugar. Toppings, such as chewy tapioca balls (also known as pearls, or boba), popping boba, fruit jelly, grass jelly, agar jelly, and puddings are often added.” It is popular in both Asian and the Western world. Though, across different regions, there are many variations in what people call this drink. This map attempts to understand those regional linguistic differences in the United States.

In 2017, the Asian American Podcast explored the “unique pearl of Asian American culture that is boba/bubble tea.” It examined its origins, people’s experiences with it, and figure out what people across the country are calling it: from boba to bubble tea and many other names in between. In preparation for this episode, the podcast released an online survey that eventually gained more than 2,000 respondents, the majority coming from the U.S. 

With the survey data, the Asian Americana Podcast was able to create this basic map:

![]({{ page.img-folder }}aNRCWBk.png)

Methods:

The podcast kindly shared the original survey data, and thus, this map interactive web map was created:
[![]({{ page.img-folder }}2QgPlX6.png)](https://bagtas3.github.io/BobaProject/examples/html/bobamap.html)

The 2 major features of the final interactive web map are the clickable pop-ups and the pie chart markers for each state. The clickable pop-ups were created with Mustache, and the pie charts were created using a Leaflet plug-in, Data Visualization Framework (DVF). 

The primary goal of the DVF library is to “simplify data visualization and thematic mapping using Leaflet - making it easier to turn raw data into compelling maps.” Examples of the potential map visualizations with DVF:
![]({{ page.img-folder }}DWcge7W.png)
![]({{ page.img-folder }}30F2vVA.png) 
![]({{ page.img-folder }}T0AcgyF.png)

The example map with 2012 election data was of particular interest because of itsuse of pie charts to display data. The code for this map was used as base for the Boba/Bubble Tea map. In order to fully remix the map with boba data, the original survey data was first aggregated to state-by-state percentages using MS Excel. Then using www.convertcsv.com, the aggregated data was converted to a JSON file. The was not converted a geoJSON format because the DVF library has a State geocoder in the code, and thus geometry was not needed.

This original data:
![]({{ page.img-folder }}30mKKVU.png)
State aggregated data:
![]({{ page.img-folder }}RZM4P1n.png)
State aggregated JSON data:
![]({{ page.img-folder }}abbfnFd.png)


Improved Interactive Map:

Heavily generalized and static, the original map did not show the nuanced state-by-state breakdown of respondents’ linguistic preferences. The interactive web map improves upon the original static map in many ways:
+ Pie charts give full detail on the linguistic preference for each state, rather than a generalization
+ It represents all answers: “Tapioca Milk Tea” and “Pearl Milk Tea” are shown, not just “Boba vs. Bubble Tea”
+ The ability to see the # of respondents in the pop-up clears up misleading information in the original map:
        + E.g. Maine had only 2 respondents, thus to say the state “strongly prefers bubble tea” is very misleading
+ Overall, allows users to make more informed conclusions on the state’s preference because all of the data is laid out clearly and in full



Sources:

SAVI 780 Final Boba Map code:
[JS](https://github.com/bagtas3/BobaProject/blob/master/examples/js/bobamap.js)
[CSS](https://github.com/bagtas3/BobaProject/edit/master/examples/css/example.css)
[HTML](https://github.com/bagtas3/BobaProject/blob/master/examples/html/bobamap.html)

Asian Americana Podcast Ep. 4:
[https://www.asianamericana.com/podcast/2017/8/22/004-bobabubble-tea](https://www.asianamericana.com/podcast/2017/8/22/004-bobabubble-tea)

Leaflet Data Visualization Framework:
* [https://humangeo.github.io/leaflet-dvf/](https://humangeo.github.io/leaflet-dvf/)
* [https://humangeo.github.io/leaflet-dvf/examples/html/election2012.html](https://humangeo.github.io/leaflet-dvf/examples/html/election2012.html)

Bubble Tea Wikipedia: 
* [https://en.wikipedia.org/wiki/Bubble_tea](https://en.wikipedia.org/wiki/Bubble_tea)
