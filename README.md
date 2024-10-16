Leaflet List Markers
============

#What
A Leaflet Control for listing visible markers/features in the map

Tested in Leaflet <s>0.7.1</s> 1.9.4

This fork:

**Examples**

<ul id="examples">
<li><a href="https://hupe13.github.io/leaflet-list-markers/examples/simple.html">Simple</a></li>
<li><a href="https://hupe13.github.io/leaflet-list-markers/examples/simple-collapsed.html">Collapsed</a></li>
<li> You can use it with WordPress, Leaflet Map and Extensions for Leaflet Map (<a href="https://github.com/hupe13/extensions-leaflet-map-testing">Testing</a>, <a href="https://leafext.de/extra/scrollable-list/">Example</a>)</li>
</ul>

**Changed**

* scrollable list
* collapse (only with click)
* new event: item-click, map update-end

<hr>

#Where

**Demos:**  
[opengeo.tech/maps/leaflet-list-markers](https://opengeo.tech/maps/leaflet-list-markers/)

**Source code:**  
[Github](https://github.com/stefanocudini/leaflet-list-markers)

![Image](https://raw.githubusercontent.com/stefanocudini/leaflet-list-markers/master/images/list-markers.jpg)

#How
Include leaflet-list-markers.css to page

Adding the List control to the map:

```
map.addControl( new L.Control.ListMarkers({layer: markersLayer}) );
//markersLayer is a L.LayerGroup contains listing markers
```
short way:
```
var map = new L.Map('map', { listMarkersControl: {layer: markersLayer} });
```

#Build

Since Version 1.4.7 this plugin support [Grunt](https://gruntjs.com/) for building process.
Therefore the deployment require [NPM](https://npmjs.org/) installed in your system.
After you've made sure to have npm working, run this in command line:
```
npm install
grunt
```
