# time_zone_map

![alt text](https://github.com/obedtandadjaja/time_zone_map/blob/master/example.png "Map example")

A simple custom map that shows different times of major cities around the world. I'm using **_Google Maps Time API_** to get the time offset of the location against GMT. Built entirely from HTML and Javascript/Jquery, but can be easily extended to use database to load the cities.

The time boxes are positioned dynamically on the map by the **_latitude_** and **_longitude_** of the city. This means that on window resize, the boxes will be positioned correctly. Because some major cities are located near each other, I also devised an algorithm to detect overlaps of the time boxes and automatically push the other down.

Live Demo: https://obedtandadjaja.github.io/time_zone_map.html

Time developing: 3 hours

## Dependencies
Jquery 1.7.2

## Copyright
Just use it but please help star the project. Thanks.
