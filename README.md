# Archeodatabank

This page in in process of editing, please, comeback later !

![logo](http://www.urieldeveaud.com/subsites/adb3/logo_archeodatabank.png)


Archeo Databank is a Geographic Information System (GIS) software running on a mobile web PHP server (USB key), made to facilitate the administration of a <b>Spatial Data Infrastructure</b> (SDI) based on History or Chronology timeline , and for publishing cartographic details and research applications .

The Archeo Databank platform is a GIS Software accessible thourgh a simple web browser. It provides numerous GIS capability and let the user do the following:

 * <b>Import/Export and store GIS data</b> (both vector and raster data)
 * <b>Query</b> Database System and external Data packages
 * <b>Publish</b> GIS data by using OGC Web Services: WMS, WFS et WMTS
 * <b>Treate, edit and style</b> data sources
 * Compose and save maps to create application projects
 * Configure and generate Web GIS applications
 * <b>Access and share maps</b>

<h3>Basic concepts: using the OGC standards</h3>

...

<h3>Main software components</h3>

...

An HTML5 Framework for Knowledge Database Visualization based on Geographic coordinates - Community Edition

> This work is a students project and it is intended to provide a dedicated template for open source GIS mapping solution. 
It is also a cross-level relational (aka matrix) and contextual data factory and archive for research and educational contents.
> It is based on Leaflet.js as map viewer, a lightweight library and its plugins. It works with GeoJson, CSV, image, local tiles, 
and vectors layers. 

### Instructions ###

> Just add this code to your HTML document header:

```html
    <link rel="stylesheet" type="text/css" href="app/galaxy-theme.css" /> // UI design
    <link rel="stylesheet" type="text/css" href="app/galaxy-views.css" /> // map, grid...
```
> Add Galaxy default setup files

```html
    <script type="text/javascript" src="app/galaxy-core.js"></script> // include dependencies
    <script type="text/javascript" src="app/galaxy-conf.js"></script> // user settings
```
> And then, connect your database...

```html
    <script type="text/javascript" src="data/layers.js"></script> // user layers def.
    <script type="text/javascript" src="data/features.js"></script> // user actions
    <script type="text/javascript" src="data/localdb.js"></script> // path to json/csv files and tiles
    <script type="text/javascript" src="data/serverdb.js"></script> // server storage connection
```
> And the last step, include the container DIV where you like, it will adjust 
to the available space in the screen or in the up-level DIV.


```html
    <div id="galaxy" class="autosize"></div> <!-- Html DIV -->
```

###THIS DOCUMENTATION IS IN PROGRESS !!!

***

![gowiki](http://www.vpul.upenn.edu/gic/images/arrow2.gif)   See documentation: https://github.com/KolamInstitute/Galaxy/wiki

====================================================

### Files structure ###

![files](http://www.kolam-institute.org/galaxy/Files_Git.jpg)

> The main application is located in its own folder, separated from the data...

### Browsers Tested ###

![browsers](http://www.webapptesting.com/wp-content/uploads/2012/12/Mobile-Browsers.jpg)

====================================================

### Test data ###

> the data provided are selected to ...

* * *
[**DATA STRUCTURE**](https://github.com/KolamInstitute/Galaxy-/wiki/Development-plan) | [**LAYERING**](https://github.com/KolamInstitute/Galaxy-/wiki/Development-plan) | [**STORAGE**](https://github.com/KolamInstitute/Galaxy-/wiki/Development-plan) | [**CORE**](https://github.com/KolamInstitute/Galaxy-/wiki/Development-plan) | [**UI**](https://github.com/KolamInstitute/Galaxy-/wiki/Development-plan) | [**MODULES**](https://github.com/KolamInstitute/Galaxy-/wiki/Development-plan)

![gowiki](http://www.vpul.upenn.edu/gic/images/arrow2.gif)   Demo app 0.6: http://www.kolam-institute.org/dev/package%20061/index.html

![gowiki](http://www.vpul.upenn.edu/gic/images/arrow2.gif)   Demo app 0.8: http://www.kolam-institute.org/galaxy/map.html

![gowiki](http://www.vpul.upenn.edu/gic/images/arrow2.gif)   Demo app 0.9: Coming soon !
* * *

**Goals (V1):**
* **Data vizualisation**: JSON/CSV ([See more details](https://github.com/KolamInstitute/Galaxy-/wiki/GeoJson-specifications))
* **Views**: Map/table
* **Screens**: desktop/tablet
* **Templates**: CSS themes and iconset

**Goals (V2):**
* **Data vizualisation**: SHP/PostgreSQL ([See more details](https://github.com/KolamInstitute/Galaxy-/wiki/GeoJson-specifications))
* **Views**: Charts/timeline
* **Screens**: smartphone

***

Dependencies 
------------

**Validator:** 
`Implemented` ![checked](http://www.digium.com/sites/digium/files/icon-green-check.png)
`Testing` ![testing](http://www.onlinecjc.ca/webfiles/images/icons/cog_add.png)
`Not yet compatible` ![notyet](http://www.whosarrested.com/images/error.png)

> The Core application includes several external libraries, 
this add new features like data searching and sorting, visualization and charting...

| Core Packages| Release | Status  | Link | Comments |
|:-------------|:-------:|:-------:|:-----|:---------|
| `Galaxy.js`  |0.9.3    |![check](http://www.digium.com/sites/digium/files/icon-green-check.png) | https://github.com/Kolaminstitute/Galaxy | UI engine |
| `Leaflet.js` |0.5.1    |![check](http://www.digium.com/sites/digium/files/icon-green-check.png) | https://github.com/Leaflet/Leaflet| Map view engine |
| `Recline.js` |0.7.0    |![testing](http://www.onlinecjc.ca/webfiles/images/icons/cog_add.png)   | https://github.com/okfn/recline | Data bind engine |
| `D3.js`      |3.0.6    |![testing](http://www.onlinecjc.ca/webfiles/images/icons/cog_add.png)   | https://github.com/mbostock/d3 | Data view engine |

> The UI is adapted to various plateforms, from desktop to mobile devices. In case of non-supported devices, it goes
to pure html template

| UI Packages  | Release | Status  | Link | Comments |
|:-------------|:-------:|:-------:|:-----|:---------|
| `JQuery.js` |0.5.1     |![check](http://www.digium.com/sites/digium/files/icon-green-check.png) | https://github.com/jquery/jquery | no comments yet |
| `JQmobile.js` |0.7.0   |![check](http://www.digium.com/sites/digium/files/icon-green-check.png) | https://github.com/jquery/jquery-mobile | no comments yet |

***

> There is a set of plugins, mostly map related, to add some extra tools

| Plugins                    | Release | Status  | Link | Comments |
|:---------------------------|:-------:|:-------:|:-----|:---------|
| `Leaflet.markercluster.js` |0.5.1    |![check](http://www.digium.com/sites/digium/files/icon-green-check.png) | https://github.com/Leaflet/Leaflet| no comments yet |
| `Leaflet.label.js`         |0.7.0    |![check](http://www.digium.com/sites/digium/files/icon-green-check.png) | https://github.com/okfn/recline | no comments yet |
| `Leaflet.geoCSV.js`        |3.0.6    |![check](http://www.digium.com/sites/digium/files/icon-green-check.png) | https://github.com/mbostock/d3 | no comments yet |
| `Leaflet.draw.js`          |3.0.6    |![testing](http://www.onlinecjc.ca/webfiles/images/icons/cog_add.png) | https://github.com/mbostock/d3 | no comments yet |
| `Leaflet.search.js`        |3.0.6    |![testing](http://www.onlinecjc.ca/webfiles/images/icons/cog_add.png) | https://github.com/mbostock/d3 | no comments yet |
| `Leaflet.hash.js`          |3.0.6    |![check](http://www.digium.com/sites/digium/files/icon-green-check.png) | https://github.com/mbostock/d3 | no comments yet |
| `Proj4Leaflet.js`          |3.0.6    |![testing](http://www.onlinecjc.ca/webfiles/images/icons/cog_add.png) | https://github.com/mbostock/d3 | no comments yet |

> The documentation is including several examples of configuration and usages.
