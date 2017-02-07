# CamoStyle [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
This is a map style that uses a publically available [Tegola](https://github.com/terranodo/tegola) extract for Bonn, Germany. It is currently still under development and is primarily styled using [Maputnik](https://github.com/maputnik/editor).

<img align="right" alt="TegolaCamoStyle" src="logo.png" />

## Viewing the map in the browser
- [Rendered with OpenLayers:](http://htmlpreview.github.io/?https://github.com/PetersonGIS/CamoStyle/blob/master/live-map.html)
Note that the water texture, road labels and tilt functionality are missing from this map, which displays the camo.json style.
- [Rendered with Mapbox:](http://www.gretchenpeterson.com/live-map-mapbox.html) 
  Note that the water texture, road labels, and tilt are working in this map, which displays the camo3d.json style. Test the tilt (pitch)   functionality by holding ctrl while clicking and dragging. The building extrusions are not yet functional on mobile devices.
- At zooms 15 and higher the data begins to appear blocky, this is due to clipping issues in the source data that are in the process of    being fixed.
- A piece of the Rhine River appears to be missing from the original data.

## Map Design

The CamoStyle basemap has a subdued color scheme to accomodate data overlays while being unique from other light basemap designs. Use camo.json for OpenLayers or mobile and camo3d.json for Mapbox implementations. Use either camo.json or camo3d.json in Maputnik for building your own style with this Tegola data extract of Bonn, Germany.

[![Camo.json map demo in a mapbox renderer](demo.gif)](http://www.gretchenpeterson.com/live-map-mapbox.html#14.66/50.7173/7.1318/-52/60)

## Editing this style in Maputnik

Editing this style to create your own style.json file is fairly straightforward. Point your browser to Maputnik at  [http://maputnik.com/editor/](http://maputnik.com/editor/), click Open > Upload and point to either camo.json or camo3d.json, which you have saved locally. Change the style to suit you, then go to Export > Download to save your newly re-styled json file locally. This can then be used in a renderer like OpenLayers or Mapbox for browser display. Note that camo.json and camo3d.json use data extracted from OSM and hosted using Tegola. You may want to explore using other open tilesets as well.
