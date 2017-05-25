# ArcGIS Story Maps
An introductory tutorial for ArcGIS Story Maps

[ArcGIS](http://www.arcgis.com/home/index.html) is a [Geographic Information System](https://en.wikipedia.org/wiki/Geographic_information_system) platform.

It has high end professional applications and functionality, but also provides a free and public online version through which geographic data can be mapped and augmented with a variety of supplementary applications.

[Here are some examples of what you can do with ArcGIS](http://www.arcgis.com/home/gallery.html#c=esri&t=maps&o=modified)

The supplementary application we're interested in today is called [Story Maps](http://www.arcgis.com/home/gallery.html#c=esri&t=maps&o=modified&f=storymaps).

Story Maps is a powerful tool that allows you to integrate an audiovisual narrative with the relevant geographic relationships between the moments of the narrative and their spatial locations.

## Table of Contents
* [About](#about)
* [Getting Started -- Creating your Basemap](#getting-started)
* [Story Maps](#story-maps)
  * [Thrusting into Story Maps -- Sharing to Initialize an ArcGIS Application](#initializing-story-maps)
* [Supplements](#supplements)

## About
Last Updated May 2017  
Created by [Paul Vieth](http://paulkelleyvieth.org/)  
University of Oklahoma Libraries

## Getting Started

ArcGIS uses the "freemium" model, so though they provide various professional versions of their platform with high functionality for a cost, they also provide free public accounts. Before we get started, go to the [ArcGIS Online](https://www.arcgis.com/features/index.html) portal and create a free public account.

When you've done that, click on the "Map" tab of the main menu. From the Arc GIS Online frontpage, you can also access a Gallery to see the potential of ArcGIS Online, or access the maps you've made under "My Content", once you've created some.

In the "Map" section, you should be taken to this screen:

![ArcGIS Mapmaker](/images/storymap01.PNG)

There are three things you can do from this screen:
* adjust the zoom level and the framing of the map
* choose a basemap
* add layers

### Basemap and Zoom
ArcGIS Online only allows preset quantum zooming, so you must use the "+/-" zoom buttons and operate within the coarse adjustments they permit.

ArcGIS Online provides 12 basemap options. The default is called "Topographic", but there are options for satellite imagery, monochromatic maps, streetmaps from [OpenStreetMap](https://www.openstreetmap.org/#map=5/51.500/-0.100), and others. Think tactically and tactfully about what you need to map to represent (and what you don't) in light of your project goals and aesthetic grammar.

### Layers
The layers are the most important component of this preparatory process. "Layers" in ArcGIS can either mean map tile sets, or smatterings of geographic data: both the quantitative data of latitudes and longitudes, but also the qualitative descriptions of what those points represent.

(Refer to the [supplements](#Supplements) section to learn how to add new tile layers (in the form of a beautiful watercolor map))

There are several ways to "lay" geographic data onto the map you've set up: click the "Add" tab from the top toolbar.

![ArcGIS Add layers menu](/images/storymap02.png)

You can import layers from the web, search for publicly accessible layers on the ArcGIS Online server, or upload a file.

ArcGIS Online can work with [KML](https://developers.google.com/kml/documentation/), [GeoRSS](http://www.georss.org/), or [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) files.

For this tutorial we're going to upload be using a crime incident dataset provided by the City of Lynchburg, Virginia. The City of Lynchburg maintains an open data portal in the spirit of administrative transparency. From the [Crime Incident page of the Open Data Portal](http://data-cityoflynchburg.opendata.arcgis.com/datasets/3c7b25e759a643cb9ef7d8caf6f5db21_0?mapSize=map-maximize&geometry=-79.841%2C37.193%2C-78.535%2C37.648), download the CSV file ("spreadsheet") of the dataset.

![ArcGiS Lynchburg Virginia Crime Incident Dataset Download](/images/storymap03.png)

Return to the ArcGIS Online Map Viewer. Click the "Add" dropdown menu and select "add layer from file." Browse for the Lynchburg, VA crime incidents dataset you just downloaded.

The basemap you created will automatically populate with datapoints from the "inci_id" column of the Lynchburg crime data (this is what we want, these points represent unique instances of a committed crime).

From here you can adjust the style of the layer under "select a drawing style" (I recommend "Counts and Amounts (Size)). After you select the style, you can change the style properties by clicking "options".

This is the process for making any map in ArcGIS online. From here we will go on to create a Story Map using the map you've just created.

## Story Maps
### Initializing Story Maps

Notice the toolbar on the right at the top of the screen.

![ArcGIS Online Save Share Print Measure Search Toolbar](/images/storymap04.png)

The measurement tool allows you to determine the area of any polygon (created by successively clicking where you want the vertices, not clicking and dragging and being limited to quandrangles); the length of any line segment, or series of non-linear but conjoined line segments (again by clicking in succession); or the latitude and longitude of point.

You can also save you map from this toolbar. Make sure you do this now before we proceed!

Initializing your map in an ArcGIS web application is unintuitive from this view.
* Click "Share" in this top-right toolbar
* Check the box to share with "Everyone (public)"
* Click the bottom-right button "Create a web app", despite the fact that it appears inactive in grey.

This will open a dialog box with access to the full suite of ArcGIS web applications, this isn't the forum to discuss all of them, especially given their specialized functionalities, but we will explore the Story Map applications.
* Click "Build a Story Map"
 * Basic
 * Cascade
 * Crowdsource (beta)
 * Journal
 * Series
 * Shortlist (beta)
 * Swipe and Spyglass
 * Tour

We're going to be working Story Map Journal during this tutorial, but I really encourage you to play around with all 8 versions.

They represent different graphical/stylistic variations on the same concept: a map (one that you've designed in the map builder above), accompanied by multimodal content presented in a set of geographic relationships to the map you provide. For "Story Map Basic", that content consists merely of a clean presentation window with a brief description of the map. Also, the "Story Map Crowdsource (beta)" requires an ArcGIS subscription, but the National Parks Service has created [a great example](https://storymaps.esri.com/stories/2016/national-park-memories/index.html) of the power and poignancy of this application.



## Supplements

### Adding a New Tile Set

You can refer to [this ESRI blog post](https://blogs.esri.com/esri/arcgis/2013/04/01/using-stamen-and-mapbox-tilesets-as-basemaps-in-arcgis-com/) for adding new tile set layers to a basemap.

Maps in online mapping platforms, such as Google Maps, OpenStreetMap, ArcGIS Online, etc., display as successions of image tiles. Each map view is a matrix of tiles and as you zoom in on the map, the tiles are replaced with new tiles with more detail, thus maintaining the map's resolution.

There are a few ways to get a basemap tile set that isn't included as one of the default 12 maps in ArcGIS online.
* To manually add a tile layer from the web, refer to the above blogpost
* The easiest is just to locate a basemap layer on the ArcGIS public server and, while logged into your ArcGIS Online account, have that basemap "Open in Map Viewer".

![ArcGIS open public map tile layer in map view](/images/storymapS1.png)
