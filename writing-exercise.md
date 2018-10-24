# Datasets vs. Tilesets
### Learn to choose the right tool for creating your custom map in Mapbox Studio

![Image of Mapbox Studio topics covered in this section](https://raw.githubusercontent.com/mayormcmatt/mb-doc-test/master/mb-topics.png)

- Mapbox maps are composed of tilesets; they are an essential part of a custom map
- Datasets are the geospatial data that underlie tilesets
- Both datasets and tilesets can be imported into Mapbox Studio, but only the former can be edited

---

## Tilesets Overview
[Tilesets](https://www.mapbox.com/studio-manual/reference/tilesets/) are the primary data format for Mapbox maps: they
are a collection of raster and vector data broken up into a grid of square tiles. Out of the box, the [Mapbox Studio style
editor](https://www.mapbox.com/studio-manual/reference/styles/) includes a number of pre-generated layers for you to use
as the basis of a custom map, starting with the default [Mapbox Streets](https://www.mapbox.com/vector-tiles/mapbox-streets-v7/) layer.

Tilesets come in a number of different file formats &mdash; KML, GPX, MBTiles, and more &mdash; that can be imported
from an external source. For more information about valid file types, check the
[uploads](https://www.mapbox.com/help/uploads/) overview.

What if a Mapbox Studio user wishes to include additional information on top of one of these tileset layers, such as the
path of an off-trail hike, a property boundry, or other unlisted points of interest, but a tileset file has not been provided? For that, a new dataset will be necessary.

## Datasets Overview
[Datasets](https://www.mapbox.com/studio-manual/reference/datasets/) are a collection of GeoJSON data either imported into
Mapbox Studio from an external source or created on-the-fly using the in-browser [dataset editor tool](https://www.mapbox.com/studio/datasets/).

The dataset editor tool takes much of the intimidation out of creating or
importing GeoJSON datasets &mdash; it validates imported data, allows for the addition of new features with point, line, and
polygon drawing tools, and more. Once you feel the dataset is sufficiently populated with features, then it is ready to
be exported as a tileset where it can be used immediately as a layer in the Mapbox studio style editor.

It is important to note that once data is converted to a tileset, it is no longer editable. To alter the tileset, modify
the dataset accordingly and export it as a new tileset.

## Example Use Cases

### Sharing landmarks along a hiking trail
Your friend has raved about hiking a favorite trail and now you have decided to try it out. Thankfully, your friend enjoys
tracking their progress on a GPS and noting where important landmarks are, so they hand off a fully annotated GPX file
of their last trip.

In this case, GPX are among the file types that can be uploaded to the [Mapbox Studio tilesets
page](https://www.mapbox.com/studio/tilesets/) and used as a tileset layer. You will be able to immediately see the
output after adding the layer to styles.

### Planning the route of a cycling event
You are helping your cycling club plan their annual century ride and need to map out the route. You have been provided a
turn-by-turn route and instructions on where aid stations might be placed.

Without a GeoJSON dataset, you will have to create your own using the dataset editor tool. Using this will give you
the line drawing tools and icons necessary to trace a route, add aid stations, and note other features for participants.

