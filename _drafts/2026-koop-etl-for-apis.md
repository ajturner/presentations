---
title: "Koop: every API is a geoservice"
source_talks: [jsgeo2014/, jsgeo2015/]
status: draft
---

<!-- Draft adapted from "Koop" (js.geo, September 2014) with context from "Esri R&D JS: Some Projects" (js.geo, October 2015). TODO notes mark places that need your own reflection. -->

At js.geo in 2014 I showed a small Node.js project we had been building in the Esri R&D Center. We described it as ETL for APIs. Today [Koop](https://github.com/koopjs/koop) describes itself as a way to "transform, query, and download geospatial data on the web."

## The problem

Lots of useful data lives behind web APIs that aren't geospatial at all: GitHub, Gists, Socrata portals, OpenStreetMap. Mapping tools wanted GeoJSON or feature services. Someone always had to write a one-off converter, and the copy went stale.

## The idea

Koop sat in the middle. A provider fetched data from a source API. Koop cached it and served it back out as GeoJSON or as an Esri FeatureService, with exports to KML, CSV, and shapefiles. The R&D build experimented with UTF grids, PNG tiles styled with CartoCSS, and vector tiles.

Because the output was a standard service, any client that could read a feature service could suddenly read GitHub, Socrata, or OSM.

## The OpenStreetMap demo

The crowd favorite was querying OpenStreetMap entirely through URLs:

```
/osm/points/state/Colorado/county/Boulder/field/amenity/cafe
/osm/points/distinct/amenity
/osm/points/state/Oregon/county/Multnomah/field/amenity/toilets
```

Every public toilet in Portland, as GeoJSON, from one URL. Pipe it into geojson.io and you have a map.

## Making Esri services readable

A year later at js.geo 2015, I picked at the other side of the problem. A raw ArcGIS FeatureServer query URL is famously long. But underneath it is a small, sensible API: a SQL `where`, a geometry filter, `outStatistics` for aggregation, and `f=geojson`. Projects like Koop and [Terraformer](http://terraformer.io) were about making that API approachable for everyone else.

## Where it went

Koop is still maintained as the open-source [koopjs](https://github.com/koopjs/koop) project.

<!-- TODO: Suggested prompts:
- What did Koop end up powering, for example Hub's federated catalog or data downloads?
- Which providers did the community build that you didn't expect?
- Is "ETL for APIs" still the right framing in a world of STAC, GeoParquet, and cloud-native formats?
-->

*Slides: [Koop at js.geo 2014](https://ajturner.github.io/presentations/jsgeo2014/) · [Esri R&D JS at js.geo 2015](https://ajturner.github.io/presentations/jsgeo2015/)*
