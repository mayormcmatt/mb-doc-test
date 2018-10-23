## Writing Exercise

Topic: the difference between Mapbox tilesets and datasets.
Purpose: to help a Mapbox Studio user determine whether to upload data as a tileset or a dataset.
Audience: a user who is new to Mapbox Studio (and is not a professional developer).

Tilesets

Tilesets are the primary data format for Mapbox maps. Whether you start with your own custom data or you create a
dataset first, converting your data into a tileset will allow you to add it to a Mapbox map and style it using the
Mapbox Studio style editor.

A tileset is a collection of raster or vector data broken up into a uniform grid of square tiles at up to 22 preset zoom levels. Tilesets are used in Mapbox libraries and SDKs as a core piece of making maps visible on mobile or in the browser; they are also the main mechanism we use for determining map views.

Tilesets are highly cacheable and load quickly. Mapbox relies heavily on both raster and vector tilesets to keep our
maps fast and efficient.

# Datasets vs. Tilesets: When and Where to Use Each

### Summary:
- Mapbox maps are composed of tilesets; they are an essential part of a custom map
- Datasets are the geospatial data that underlie tilesets
- Both datasets and tilesets can be imported into Mapbox Studio, but only the former can be edited

...

Out of the box, the [Mapbox Studio style editor](https://www.mapbox.com/studio-manual/reference/styles/) includes a
number of pre-generated layers for you to use as the basis of a custom map, starting with the default [Mapbox
Streets](https://www.mapbox.com/vector-tiles/mapbox-streets-v7/) layer. These layers are composed of
[Tilesets](https://www.mapbox.com/studio-manual/reference/tilesets/): a collection of raster and vector data broken up
into a grid of square tiles.

What if a Mapbox Studio user wishes to include additional information on top of one of these tileset layers such as the path of an off-trail
hike, an property boundry, or unlisted points of interest? Users can generate their own tilesets from [Datasets](https://www.mapbox.com/studio-manual/reference/datasets/), a collection of GeoJSON data either imported into
Mapbox Studio from an external source or created on-the-fly using the in-browser [dataset editor
tool](https://www.mapbox.com/studio/datasets/). The dataset editor tool takes much of the intimidation out of creating or
importing GeoJSON datasets &mdash; it validates imported data, allows for the addition of new features with point, line, and
polygon drawing tools, and more.