find-a-bike-train
=================

Schedule bike routes are popping up. Which one should you join?

## goal

Here is an [outline of an ideal
search](https://gist.github.com/monking/c0f68340eba759258d4b), and here is
another outline of the first steps we plan to take towards that goal:

1. Given start and end lat/lng coordinates, rank routes by proximity and
   direction.

2. If any conductors are actively tracking their train, show it on the map in real time.

3. Store the start end points as entries in a survey, and prompt for more info
   if the user doesn't find a satisfactory route.

## stack

### server

- Ruby on Rails
- PostgreSQL + PostGIS

### web client

- angular.js

### native mobile client (later)

- cordova (phonegap) wrapping web client

## tracking

Currently our conductors are using Geotracks for Android, and Geotrigger for
iOS, to track. Though its battery usage is excellent, at some stage we will
implement a basic tracking app in JavaScript using cordova.
