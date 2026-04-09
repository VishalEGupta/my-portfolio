# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Personal portfolio for Vishal Gupta. Single `index.html` — no build step, no dependencies, no package manager. Deployed via GitHub Pages at `https://vishalegupta.github.io/my-portfolio/`.

## Development

```
open index.html
# or
python3 -m http.server 8080
```

## Design intent

Dark minimal aesthetic (`#0f0f0f` background). Reference: [mhouge.dk](https://mhouge.dk) — understated, not resume-like. Avoid anything that reads as a traditional resume layout: no skill bars, no timelines, no icon grids. Let whitespace and typography do the work.

## Architecture

Everything is in `index.html`: structure, styles (in a `<style>` block in `<head>`), and content. CSS uses custom properties on `:root` for the color palette. Sections: `#hero`, `#projects`, `#about`, `#contact`. Nav uses fragment anchors with `scroll-behavior: smooth`.

`resume.pdf` is served from the same directory and linked from the about section.

Do not split into separate files or introduce a build pipeline unless explicitly asked.
