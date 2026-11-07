---
title: "Geographic doesn't mean cartographic: chatbots, voice, and civic data"
source_talk: sonar/
status: draft
---

<!-- Draft adapted from "Chatbots as an Interface for Spatial Data and Analysis" (Esri R&D DC, June 2017). TODO notes mark places that need your own reflection. -->

In 2017 I gave a talk with a deliberately provocative premise for a room full of geographers: the map is not always the right interface.

Maps are wonderful at showing structure. They take many forms, from 3D-printed terrain to Marshall Islands stick charts that encode ocean swells in bent sticks and shells. But that last example makes the point. **Geographic doesn't mean cartographic.** Some of the oldest navigation tools carry spatial knowledge without anything we would call a map.

## Why it matters for public data

Geographic information systems manage public, physical infrastructure: streets, pipes, trash routes, parks. That infrastructure supports communities, and communities are made of people with very different perspectives, skills, and devices.

If we want data-driven citizenship, public digital infrastructure has to be accessible. It has to meet people where they are. For a lot of people, the question isn't "show me a map of service areas." It's "what's going on around me?"

## Sonar: talk to your infrastructure

[Sonar](https://github.com/esri/sonar) was our experiment in answering that question conversationally. Residents could ask about trash pickup, recycling, or recent crime through Slack, Facebook Messenger, or Amazon Alexa.

Under the hood it was small pieces, loosely joined:

- Sonar.js and Claudia.js running as AWS Lambda functions behind API Gateway, plus Alexa skills.
- ArcGIS geocoding, routing, and GeoEnrichment to turn an address into context.
- Ordinary web maps acting as a voice interface. A popup template like "Trash pickup is {FREQ_REFUSE} and recycling is {FREQ_RECYCLING}" becomes a spoken answer.

You can see it working in the [DevSummit 2017 plenary demo](https://youtu.be/H_cdn2kVB-E?t=4m35s) and the [architecture walkthrough](https://youtu.be/1J5y8sJ9aKI).

## What we learned

**Design for humans, not schemas.** Public datasets say "Mon," "Thu," and "Thurs." A screen reader or a voice assistant needs "Monday" and "Thursday." Most of the work was cleaning data into language.

**Discoverability fights predictability.** A map shows you everything at once. A conversation only answers what you think to ask. Scripted bots are predictable but narrow. AI-driven bots are flexible but can surprise you.

**Privacy and accessibility are design inputs, not afterthoughts.** Asking "what's around me" means sharing where "me" is.

**Only add voice if it makes the product better.** That was the line in my speaker notes, and it still holds.

## Looking back from 2026

<!-- TODO: This is the section that makes the post worth reading today. Suggested prompts:
- In 2017 the "AI bot" option was the risky one. Large language models flipped that. What does Sonar look like rebuilt on an LLM with tool calls into ArcGIS services?
- Which of the lessons above held, and which turned out wrong?
- How does this connect to how Hub and civic data portals expose data to AI assistants now?
-->

*Slides: [Chatbots as an Interface for Spatial Data and Analysis](https://ajturner.github.io/presentations/sonar/)*
