---
layout: post
title:  "Country dragging with GMaps"
permalink: yomap
date:   2014-01-01 10:06:00
categories: code
---

<b>Update 2014-08-10:</b> Added US States and Cities.  Not a good time.

I love to explore Google Maps, and I've always wanted to be able to drag countries around to compare sizes, so I created [http://shmay.github.io/yomap/][1]

GMaps has a 'geodesic' property that enables polygons to correctly resize as they are dragged around the world!  Before this, I didn't realize that flat maps displayed skewed country sizes to compensate for what would normally be a spherical globe.

At first glance, the countries far from the equator look massive.  However, drag Russia
near the equator and suddenly it's hardly bigger than Brazil.  Antarctica is tiny!  DR Congo amazingly dwarfs Europe.

The hardest part of this project was getting the country polygon coordinates in decimal degrees.  I spent a couple days trying before
finally [posting on StackExchange][2] and promptly receiving an easy solution!  God bless SO/SE.

Ultimately I used [Natural Earth's][3] data, though it's so detailed that dragging countries can get a bit computationally expensive.  It's also far too precise for my purposes -- it gives multiple polygons for a country where only one or a couple would be ideal.

Stuff to add:

* optionally drag entire countries, not just polygons
* urls that represent the current state of the map, so you can link to the map you've created

[1]: http://shmay.github.io/yomap/
[2]: http://gis.stackexchange.com/questions/81559/polygon-country-boundaries-in-decimal-degrees
[3]: http://www.naturalearthdata.com/
