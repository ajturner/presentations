# Talks by Andrew Turner

Slides from talks on open data, open source, web mapping, and civic technology, 2013–2017.

**Browse them at [ajturner.github.io/presentations](https://ajturner.github.io/presentations/).**

## Layout

- Each talk folder is a self-contained deck (reveal.js, big.js, or a Keynote HTML export).
- `pdf/` holds a PDF of every deck for quick skimming.
- `thumbs/` holds the title-slide images used on the homepage.
- `shared/reveal-devsummit-2016/` is the reveal.js build shared by the two 2016 DevSummit decks.
- `_drafts/` holds unpublished blog post drafts adapted from the talks. GitHub Pages does not publish this folder.

## Regenerating PDFs

reveal.js decks print directly from the browser:

```
chrome --headless --print-to-pdf=pdf/<talk>.pdf "http://localhost:8000/<talk>/index.html?print-pdf"
```

The big.js and Keynote decks have no print mode, so their PDFs are assembled from one screenshot per slide.
