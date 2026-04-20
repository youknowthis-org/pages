# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static HTML website for YouKnowThis — a landing page plus legal documents (privacy policy, terms of service). No build tools, no dependencies, no compilation step.

## Development

Open HTML files directly in a browser or serve them with any static file server:

```bash
python3 -m http.server 8080
```

## Architecture

All pages are self-contained HTML files with inline styles. Shared assets live in `images/`.

- `index.html` — Landing page with logo and links to legal docs and contact email (office@fuchs.sh)
- `privacy.html` / `terms-of-service.html` — Legal documents (generated from a template tool, not hand-authored)
- `images/logo.svg` / `images/fav.svg` — Identical SVG used as logo and favicon

**Branding:** Primary color `#362C66` (purple), Heebo font from Google Fonts (weights 400, 500, 700).

## Commit Convention

Use `NO-TICKET` prefix for commits not tied to an issue, e.g.:
```
chore: NO-TICKET Add index
```
