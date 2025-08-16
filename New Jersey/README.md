# Maps for the state of New Jersey

## General

These are maps that generally come from the New Jersey Department of Environment Protection,
specifically the [Bureau of Geographic Information Systems](https://dep.nj.gov/gis/)
and [Division of Fish and Wildlife](https://dep.nj.gov/njfw/destinations/maps/).
Some of this data is published for the hunting, fishing, and trapping communities in New Jersey.

## Source of the Data

New Jersey publishes the data using ArcGIS technology. These are the main pages where you can
find the map data endpoints. These map data endpoints can usually be used to import the maps
into CalTopo. Note that some of the map data endpoints here do not work with CalTopo at all, some
do not work well, though most of them work fine.

* https://njdep.maps.arcgis.com/home/gallery.html
* https://gisdata-njdep.opendata.arcgis.com/
* https://mapsdep.nj.gov/arcgis/rest/services/Features

## Map Layer Types

Two types of custom map layers that CalTopo supports are:
* [Custom Sources](https://training.caltopo.com/all_users/base-layers/custom-source)
* [WFS Sources](https://training.caltopo.com/all_users/base-layers/wfs)

Some of the New Jersey map data is best imported as a Custom Source,
others as a WFS Source. In some cases, the New Jersey data can only
be imported as one or the other. The type a specific map should be
imported as was determined by what data can be displayed, how fast
CalTopo can render the data, and the visual appeal of the rendered data.

To create custom map layers, follow the instructions found in the
documentation links above. The below information will not tell you
how to do it, it will only provide the data you need to enter into
the relevant CalTopo entry fields.

_Note that the "Auto-Configure URL" field is never set - leave that
empty when creating one of the map layers below. You do not need it
because the data below is supplying the configuration you need._

## Custom Sources

There are two important piece of data you need to know when creating one of these Custom Sources:

* `URL Template`: a very long URL that you must copy exactly
* `Type`: should always be set to `WMS` unless otherwise specified

The other fields are dependent on user preferences. You decide what you want:

* `Name`: the names below are just suggestions, you can name your map layers anything you want
* `Max Zoom`: maximum zoom level in which the data is displayed - the value of this field may be restricted by the map itself
* `Overlay?`: determines if you want the map layer to be a base layer or an overlay. It is up to you what you want to use, though a map may not render properly as one over the other. Refer to the CalTopo documentation for why you would want to choose one over the other.

----

* NJ Black Bear Zones
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:18
* NJ Deer Zones
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:17
* NJ Shellfish Leases
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:39
* NJ Special Winter Canada Goose Season Zones
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:14
* NJ State Parks and Forests
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Applications/DEP_Trails/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:18
* NJ State Parks and Forests Trails
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Applications/DEP_Trails/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:0
* NJ Turkey Zones
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:12
* NJ Upland Bird Stocking Areas
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:28
* NJ Waterfowl Zones
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:11
* NJ WMA Roads
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Transportation/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:23
* NJ Woodcock Zones
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/export?dpi=96&transparent=true&format=png32&bbox={left},{bottom},{right},{top}&bboxSR=EPSG:3857&imageSR=EPSG:3857&size={tilesize},{tilesize}&f=image&layers=show:10

## WFS Sources

There are two important pieces of data you need to know when creating one of these WFS Sources:

* `URL Template`: a very long URL that you must copy exactly
* `Label Name`: the name of one of the labels in the map data set; each data point's label value is what CalTopo will show on the map when labeling each of the map's data points

The other fields are dependent on user preferences. You decide what you want:

* `Name`: the names below are just suggestions, you can name your map layers anything you want
* `Min Zoom`: minimum zoom level in which the data is displayed - the value of this field may be restricted by the map itself

----

* NJ Deer Management Units
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Grids/MapServer/26/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: DMU
* NJ Public Access Locations
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/7/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: PA_ID
* NJ Saltwater Fishing Access Sites
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/31/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: SITE_NAME
* NJ State Parks and Forests Parking
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Applications/DEP_Trails/MapServer/30/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: FEATURE_NAME
* NJ Trout Stocked Lakes
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/36/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: WATERBODY
* NJ Trout Stocked Streams
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/35/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: NAME
* NJ Trout Stocked Streams (Midpoints)
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Environmental_admin/MapServer/34/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: NAME
* NJ WMA
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Land/MapServer/65/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: FEE_SIMPLE_NAME
* NJ WMA Parking / Ramps
  * URL Template: https://mapsdep.nj.gov/arcgis/rest/services/Features/Land/MapServer/62/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: FEATURE_NAME
* NJ WMA Restrictions
  * URL Template: https://services1.arcgis.com/QWdNfRs7lkPq4g4Q/arcgis/rest/services/Wildlife_Management_Area_WMA_Restrictions_in_New_Jersey/FeatureServer/41/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: CATEGORY
* Wharton State Forest Visiting Vehicle Use Roads
  * URL Template: https://services1.arcgis.com/QWdNfRs7lkPq4g4Q/arcgis/rest/services/Wharton_State_Forest_Visiting_Vehicle_Use_Roads/FeatureServer/19/query?where=1%3D1&f=geojson&geometry={left},{bottom},{right},{top}&geometryType=esriGeometryEnvelope&spatialRel=esriSpatialRelIntersects&inSR=4326&outSR=4326&outFields=*&returnGeometry=true
  * Label Name: PRIME_NAME
