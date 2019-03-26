---
layout: project-page
title: "Baseball Stadiums of New York City Past & Present"
linkname: baseball-stadiums-of-new-york-city-past-present
author: "Danny Goodman"
tagline: "This draft project maps and details the current and historic baseball stadiums of New York City, complete with historical information and photographs."
location:
    - place: New York, NY, USA
project-link:
    - href: https://ddouglasgoody.github.io/nyc-baseball-stadiums/
tags:
    - tag: baseball
    - tag:  stadiums
    - tag:  city
    - tag:  historic
thumbnail-path: img/baseball-stadiums-of-new-york-city-past-present/roiRRLQ.png
img-folder: ../../img/baseball-stadiums-of-new-york-city-past-present/
timestamp: 3/24/2019 11:47:16
---
The purpose of this project, really, is to indulge my love of both baseball and nostalgia. When I moved to New York City almost two decades ago, I became enamored with the history sitting alongside the ever-changing present. I enjoy going to baseball games, not simply for the sport, but for the history living in these stadiums. In looking back at stadiums of the past, I've found myself drawn in to what the city might have looked like when these arenas of sport existed.

Overall, my goal for this map and webpage is simple: to show both the current and a select group of historic stadiums throughout New York City. These stadiums include both major and minor league teams, as well as [other professional leagues](https://www.britannica.com/sports/Negro-league).

I made the data for this project myself, using QGIS. The data was built into a shapefile, which I then converted to a GeoJSON to include in the web map.

![]({{ page.img-folder }}tet2hgA.png)

The properties include the stadium name, team or teams that called the stadium home, the date built (and, if applicable, end of use), and a “status” of historic or current (used mostly to change the symbology on the map).

![]({{ page.img-folder }}7IepQB2.png)

In addition, there is a photo url attribute, which links to photograph or representative picture stored on the project GitHub page.

![]({{ page.img-folder }}FgXr5Xk.png)

I used a variety of web resources to track down both information and photographs of these stadiums, past and present. The majority of the information came from [BrooklynBallParks.com](http://brooklynballparks.com/), with additional information and mapping assistance coming from [NYCityMap](http://maps.nyc.gov/doitt/nycitymap/), [Wikipedia (I know, I know)](https://www.wikipedia.org/), and [CBS Sports](https://www.cbssports.com/). The basemap was made using [Mapbox](https://www.mapbox.com/).

![]({{ page.img-folder }}XUwAEzm.png)

The interface of the map is simple - users can move around New York City, and clicking on a dot produced a sidebar of information (taken from the attribute table, using mustache).

![]({{ page.img-folder }}HfkzobZ.png)

In the bottom right corner of the map, too, there is an "About" button, which when clicked brings up the source information for the map.

![]({{ page.img-folder }}PvAHugB.png)

As I continue to work on this map beyond this class, I aim to, firstly, solve several ongoing issues. Once those are tackled, I would love to enhance the design of the page, particularly in its lack of CSS attractiveness. I have spent time looking at other websites, and I hope to bring some complexity, design-wise, to the user experience. In addition, I would like to add some details, such as sounds (perhaps the sound of a bat hitting a ball, a crowd cheering, when the user clicks on a feature), and even enhance the data with modern photographs and information showing what these historic sites look like now (if no longer in use as a stadium). A coworker suggested a digital walking tour of these stadiums could be housed on this site, building off of what is there and could be added.
