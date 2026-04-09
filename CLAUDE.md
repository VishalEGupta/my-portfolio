# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Single-file static portfolio website. All HTML, CSS, and any future JS lives in `index.html` — no build step, no dependencies, no package manager.

## Development

Open directly in a browser:
```
open index.html
```

To preview with live reload (if needed):
```
npx serve .
```

## Architecture

Everything is in `index.html`: structure, styles (in a `<style>` block in `<head>`), and content. CSS uses custom properties defined on `:root` for the color palette. Sections are `#hero`, `#projects`, `#about`, `#contact`. The nav links use fragment anchors with `scroll-behavior: smooth` on `html`.

Keep it this way — do not split into separate files or introduce a build pipeline unless explicitly asked.
