---
title: "From open data to data infrastructure: 2013–2017"
source_talks: [hesn/, opendata/, esri-devsummit-2016/, ds-2016-od-customization/]
status: draft
---

<!-- Draft combining four talks: "Open Data for Innovation" (USAID HESN, November 2013), "Open Data" (Esri DC, March 2014), and the two "ArcGIS Open Data for Developers" talks (Esri DevSummit, March 2016). TODO notes mark places that need your own reflection. -->

Between 2013 and 2016 I gave a series of talks about open data. Read together, they trace how an idea about transparency became a piece of public infrastructure.

## 2013: What makes data open?

For a USAID audience in 2013 I started with a definition. Open data is free or nearly free, accessible, machine-readable, licensed for reuse, and timely.

The economic case was big. McKinsey estimated that [open data could unlock more than $3 trillion a year](https://www.mckinsey.com/capabilities/mckinsey-digital/our-insights/open-data-unlocking-innovation-and-performance-with-liquid-information) across just seven sectors. Its most striking finding was that about one-third of that value comes from benchmarking: simply being able to compare.

The examples were already real. USAID published a developer portal. Volunteers mapped Kibera in OpenStreetMap. The World Bank's Mapping for Results put aid projects in Uganda on a map next to health and transport data.

## 2014: Don't move your data

A year later the principles had sharpened into four words: discoverable, explorable, accessible, collaborative.

The key technical idea was **don't move your data**. Governments already had authoritative data in their own systems. Copying it into a separate portal created stale duplicates. Instead, tools like Koop could translate between formats on the fly, so a school facilities GeoJSON file could become a feature service and then a web map without anyone exporting anything.

That idea became ArcGIS Open Data.

## 2016: Open data for developers

By the 2016 Esri Developer Summit, ArcGIS Open Data was a platform with hundreds of sites, including Washington, DC, Iowa DOT, Delaware, and the Department of Homeland Security.

The developer story had grown up too:

- A JSON API following the JSON API standard, so the catalog itself was programmable.
- Federated search, so a city's data.json fed straight into Data.gov.
- Koop and Winnow for converting and querying data from other platforms like Socrata.
- Open-source starter apps in Ember, React, and Angular.

The last slide was titled "Road Ahead," and it showed the first Hub sites from Los Angeles, the Association of Washington Cities, and Denton, Texas.

## What happened next

ArcGIS Open Data became ArcGIS Hub the following year.

<!-- TODO: This is the payoff section. Suggested prompts:
- How did "data-driven citizenship" from the 2016 deck shape what Hub became?
- Which ideas held up, like "don't move your data," and which didn't?
- What is the open data movement's biggest unfinished business in 2026?
-->

*Slides: [Open Data for Innovation](https://ajturner.github.io/presentations/hesn/) · [Open Data](https://ajturner.github.io/presentations/opendata/) · [ArcGIS Open Data for Developers](https://ajturner.github.io/presentations/ds-2016-od-customization/)*
