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

# Datasets vs. Tilesets: The Essentials

Out of the box, the Mapbox Studio style editor includes a number of pre-generated layers for you to use as the basis of a custom map,
starting with the default [Mapbox Streets](https://www.mapbox.com/vector-tiles/mapbox-streets-v7/) layer. These layers
are comprised of [Tilesets](https://www.mapbox.com/studio-manual/reference/tilesets/): a collection of raster and vector
data broken up into a grid of square tiles.

What if a Mapbox Studio user wishes to include additional information on top of one of these layers such as the path of an off-trail
hike, a property boundry, or unlisted points of interest? Users can create and import their own tilesets from
[Datasets](https://www.mapbox.com/studio-manual/reference/datasets/), a collection of GeoJSON data either imported into
Mapbox Studio from an external source or created on-the-fly using the [dataset editor tool](https://www.mapbox.com/studio/datasets/).