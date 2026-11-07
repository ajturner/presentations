---
title: "The nuts and bolts of open"
source_talk: aag2014/
status: draft
---

<!-- Draft adapted from "OpenGIS: Technical Issues" (AAG Annual Meeting workshop, April 2014). The deck is mostly single phrases over images, so this draft expands each phrase into a paragraph. Check each one against what you actually meant. -->

At the 2014 AAG meeting I was asked to cover the technical side of "open GIS." The talk boiled down to a handful of principles. Most of them are still how I think about building geospatial systems.

## There's more to open than source code

Open means at least four things: source code, specifications, data formats, and licensing. A project with open code but a proprietary format isn't really open. Neither is an open format with a license that forbids reuse.

## Pragmatism beats purity

There's an XKCD comic about how fourteen competing standards inevitably become fifteen. Technology changes faster than any organization can standardize it. The formats that win are usually the ones that are easy to use today, like GeoJSON, not the ones designed by committee for every future case.

## Complexity grows; plan for it

Every system accumulates complexity, and entropy is inevitable. Niche interests pile up features. Meanwhile there are new developers every day who need to get started without reading a specification first.

## Let people under the hood

Tools should let people look inside, understand how they work, and change them. That is the difference between a tool for people and a black box.

## Small pieces, loosely joined

David Weinberger's phrase describes the web, and it describes good GIS architecture too. Instead of one monolith, build small components that each do one thing and connect over HTTP. Favor flexibility over a perfect ontology, and folksonomy over a rigid taxonomy when users need to describe their own data.

## Hybrid architectures

The practical result is hybrid systems: commercial and open-source parts that are interchangeable because they speak the same open protocols. That is how Esri approached open source, with 718 GitHub members and 376 repositories by the time of this talk.

## Still true?

<!-- TODO: Your current view. Suggested prompts:
- GeoJSON won. What's the next "pragmatic" format: GeoParquet, PMTiles, cloud-optimized GeoTIFF?
- Did "small pieces loosely joined" survive the move to cloud platforms and SaaS?
- What does "let me under the hood" mean when the component is an AI model?
-->

*Slides: [OpenGIS: Technical Issues](https://ajturner.github.io/presentations/aag2014/)*
