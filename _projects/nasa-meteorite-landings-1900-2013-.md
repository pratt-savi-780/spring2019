---
layout: project-page
title: "NASA Meteorite Landings (1900 - 2013)"
linkname: nasa-meteorite-landings-1900-2013-
author: "Hector Hernandez"
tagline: "The interactive web map displays about a century's worth of meteorite landing data from the NASA Open Data Portal. Data on this map can be filtered by year from a drop-down menu. The interest in making this map was to see what the trend of meteorite landings has been over time and where they tend to land."
location:
    - place: Worldwide 
project-link:
    - href: https://glitch.com/~780-finalprojecthh031719
tags:
    - tag: NASA
    - tag:  meteorite landings
    - tag:  meteorites
    - tag: 
thumbnail-path: img/nasa-meteorite-landings-1900-2013-/5lisv5O.png
img-folder: ../../img/nasa-meteorite-landings-1900-2013-/
timestamp: 3/24/2019 16:47:03
---
The NASA meteorite landings interactive map was used as a starting point to research this topic. There are several questions that arise with such a topic. Where have meteorites tended to land over time? Have these meteorites landed in densely populated or developed areas? How often do meteorites land on earth? Below is map I found interesting and helped me get started on this project.

![]({{ page.img-folder }}EkEMQYf.png)

The data for the map was obtained from the NASA Open Data Portal and the API endpoint with filtering was used to retrieve the data and display it on the web map. The dataset has about 10 fields that include year, mass, and name of meteorite. The years of the dataset are 1900 -2013. It is important to note that the dataset has about 35 thousand records but there are several hundred records with no values for their lat and long fields. As a result these specific values with no lat and long would not be displayed on the map. The focus of the project was to create drop down menu for a user to select a year to display meteorite data. The select element and option elements for all the years 1900 – 2013 were added into the html code. In the javascript an event listener was added so that every time the dropdown menu changed with a selection of a year, the function loaddata was run to display only data for the specific year selected. See screenshot of html and javascript below.

![]({{ page.img-folder }}ENPL4hl.png)

![]({{ page.img-folder }}dhU9dvz.png)

The rest of the code in html/javascript consisted of creating a sidebar with text, a link, and the dropdown menu. A few plugins were added for searching for a location, a dynamically changing scale bar, and a marker cluster group plugin that groups markers together based on proximity/zoom level.  Map options were also used to bound the map by zoom level and maximum extents. Most styling was done with selectors in the CSS code. A Mustache template was used to style the text inside the pop—ups. See image below of map.

![]({{ page.img-folder }}5lisv5O.png)

Some issues of this project included knowing what bits of code to keep inside the loaddata function and which not. For example, initializing the marker cluster group plugin outside of the function allowed the code to work with no issues. Also, clearing the data and markers each time the function was run was important so that we don’t get multiple selections of data appearing on the map. Using sublime to fix indentation was very helpful to fix any issues with the indents.
Using the developer tools was invaluable as it helped me figure out issues with the code and also assisted me in styling with CSS. Mustache for styling for the pop-up text and utilizing variables to simplify the code was also very helpful.
As next steps, I would like to figure out why some records are missing lat and long, and why there are so many records at Null Island or Antarctica. These records may need to be omitted, possibly with filtering. Using different sizes of the markers based on mass of the meteorites is also a possibility. I want to continue to work on this map to answer questions like are the meteorites landing in densely populated and developed areas.
