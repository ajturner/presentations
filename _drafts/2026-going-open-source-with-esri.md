---
title: "Castles in the air: why a GIS company went open source"
source_talk: esri-opensource/
status: draft
---

<!-- Draft adapted from "Going Open-Source with Esri" (January 2013), mostly from its speaker notes. TODO notes mark places that need your own reflection. -->

In early 2013 I gave a talk explaining why Esri, a company known for a robust and commercial platform, was going to start building in the open. Rereading the notes now, the argument still holds up, and the results are easier to measure.

## No platform can serve every community

ArcGIS is built to be stable, secure, and scalable for complex problems. But each community that uses it, from governments and militaries to NGOs, planners, and journalists, has its own methods, requirements, and language. No product team can build every specific feature. Users need tools that speak their language, without having to learn esoteric technical terms.

## Programmers build castles in the air

Fred Brooks wrote that the programmer "builds his castles in the air, from air, creating by exertion of the imagination." Anyone who has written even a small script knows that feeling. The tools to imagine something and ship it to millions of people already exist.

Open source is how you give that power to the communities you can't serve directly.

## Freedom, like Lego

Many of us grew up with Lego kits. We built the pirate ship once, admired it, and then took it apart and mixed the pieces into something new. Some creations stayed together for years and became parts of larger ones.

That is what a good platform should feel like: well engineered, stable, and fun to remix. Open source gives people the freedom to choose, to innovate, and to evolve their own solutions.

## This wasn't new, but this time was different

Esri had long used and supported open technology: PostgreSQL, GDAL, OpenStreetMap, OGC standards, Python. The web had already made "view source" the default way developers learn from each other.

But publishing isn't collaborating. We had done resource centers and code samples before. This time the point was **positive feedback loops**: Apache 2 licensing by default, real engineers working in public, and contributions flowing both ways.

## Cathedral and bazaar

Eric Raymond framed open source as the bazaar replacing the cathedral. I argued it's a hybrid. The cathedral provides inspiration, structure, and a place to gather. The bazaar provides communication and self-organization. A company can be both.

## What happened next

When I gave this talk, Esri had nearly 50 public repositories and about 76 engineers on GitHub. By my AAG talk a year later, it had 718 members, 376 repositories, and 3,324 forks.

<!-- TODO: Bring this up to date. Suggested prompts:
- How many repositories and contributors does Esri have on GitHub today?
- Which projects from that era became load-bearing: Koop, Terraformer, Calcite, Leaflet integrations?
- What did open source change inside Esri's culture, beyond the code?
- What would you tell a company starting this journey in 2026?
-->

*Slides: [Going Open-Source with Esri](https://ajturner.github.io/presentations/esri-opensource/)*
