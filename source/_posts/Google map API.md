---
title: Google Maps API & related
author: Tiffany Gu
tags: ["Google Maps API", "JavaScript"] 
categories: ["JavaScript", "Firebase"]
---

# Wrote in Jan 2020 for BCIT Hackathon.
<!-- wp:paragraph -->
<p>This weekend we went to QDS Hackathon about data analysis. We decided to collect data from public database and plot them on the map. We chose Google Maps as our platform. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>The APIs for Google Maps are extensive, but the service actually costs money. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>In Google Maps, it uses the coordinates to identify a certain location. That is, we need latitude and longitude to spot a marker on the map. One challenge for us is to convert the data from address to coordinates. Since Google services can actually cost money, one of the challenges for us was to find a way that saves money. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>*Google services give $300 of free credits. Geocode gives $200 of free credits. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Geocoding</strong></p>
<!-- /wp:paragraph -->

![Snippet of code getting coordinates](https://i.imgur.com/fUhh83N.png)

<!-- wp:paragraph -->
<p>results[0].geometry.location this is a string returning (xxx.xxxx, xxx,xxxx). If you want the floating numbers, you need to parse it into two substrings and parseFloat the two substrings. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Shapes: circles</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>center: {lat: parseFloat((results[0].geometry.location).toString().substring(1,11)),lng:parseFloat((results[0].geometry.location).toString().substring(12,25))}</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>If you are trying to get the coordinates from geocoding, you need to process the data using the method mentioned above. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p><strong>Shapes: rectangles</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>This uses bounds. </p>
<!-- /wp:paragraph -->

![Random squares on a map](https://i.imgur.com/WdTJHSw.png)

<!-- wp:paragraph -->
<p><strong>Customize markers</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>You can add attributes to the marker icons. You can also add customized icons.</p>
<!-- /wp:paragraph -->

![Icon attributes](img/image-3.png)

---
Link to the project: [click me](https://qds20team16.web.app/).

---
v.1 2020.1  

v.2 2020.7  

v.3 2020.8

v.4 2020.8 --fixed the image links + author name  

v.5 2020.9 -- grammar fixes