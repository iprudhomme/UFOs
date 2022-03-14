# UFOs
## Overview
for our 11th data analytics project.  We created a dynamic website using javascript, bootstrap, css, and d3 to create a searchable UFO siting website.  Given a list of many reported UFO sightings, we created a table in javascript and then utilized values from input boxes to apply filters on the data so people can find information on the sightings in the area of their choice.
## Results
The site welcomes visitors who may be interested in looking up sightings based on a given city, state, or country.  As well the user can filter the list by the shape of the UFOs.  Perhaps a user saw something strange and wanted to see if anyone near them had seen something similar.  The sight works by just changing the inputs under "Filter Search".   
![Filter Search](./static/images/filter%20boxes.png)

Once the user leaves the input box and clicks on another box or somewhere else on the site, the javascript code will recognize the change and re-filter the data.  Of a user clears the data, then the filter gets removed when they move on to another element on the page.  Say I lived in "el cajon, CA".  I could add "El Cajon" to the state input box and "CA"  filter directly on city and I would find 5 other sightings in the area.  Or I could filter on state for "CA" and I could find 20 sightings.  

![UFO WebSite](./static/images/ufosighting.png)
## Summary
A drawback of this design is that the user must type in the exact search criteria to match.  I limited this drawback by at least converting the search values to the list values using lowercase.  This way both "CA" and "ca" would match.  Even still, the user must know the exact city of the search or get the entire state.  Perhaps a proximity search, which calls external APIs to determine the distance between a filter city and the cities in the list so the user can filter on cities within X miles of the request city.  Also, it would be nice if they user could have a spot to post their own UFO sighting, thus allowing the information in the site to grow over time.  