# time_zone_map

![alt text](https://github.com/obedtandadjaja/time_zone_map/blob/master/example.png "Map example")

A simple custom map that shows different times of major cities around the world. I'm using **_Google Maps Time API_** to get the time offset of the location against GMT. Built entirely from HTML and Javascript/Jquery, but can be easily extended to use database to load the cities. Note that API calls are made every hour instead of every minute because Google limits the number of API calls a day (for free versions).

The time boxes are positioned dynamically on the map by the **_latitude_** and **_longitude_** of the city. This means that on window resize, the boxes will be positioned correctly. Because some major cities are located near each other, I also devised an algorithm to detect overlaps of the time boxes and automatically push the other down.

The code that I am posting here is obviously different from the one I developed for work for simplicity and extensibility sake (everyone has different needs, and the one I made for my work is very specific to our needs and what environment is available to us). For work, I coupled this HTML page with a C# backend to grab the cities from a database and set the application to check if there are new cities in the database every hour. On top of that I also built a Windows Service that runs every hour to call the API and populating the values to the database. The reason being this application will be used by 200+ people in the company and that I cannot have them call the API every time they open the application, and every hour they keep the application open. Yes, I am saving my company some money by doing this (free versions have limited API calls). This is just one example of how this HTML/Jquery page can be extended.

Live Demo: https://obedtandadjaja.github.io/time_zone_map.html

Time developing: 3 hours

## Dependencies
Jquery 1.7.2

## Copyright
Just use it but please help star the project. Thanks.
