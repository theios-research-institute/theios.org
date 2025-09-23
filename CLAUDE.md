# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the theios.org landing page repository - a static website for the Theios Research Institute. The site serves as the public-facing presentation for the research institute and provides links to related resources including GitHub organizations and the codex.nexus website.

## Architecture

- **Static HTML site**: Single-page application with embedded CSS and JavaScript
- **Styling**: Inline CSS with custom properties for theming (dark/light/auto modes)
- **Theme system**: JavaScript-based theme toggle with localStorage persistence
- **Responsive design**: Mobile-first approach with CSS grid and flexbox
- **Typography**: Mixed font stack (Inter for UI, Merriweather for content)
- **Assets**: Logo variants, favicon, and minified CSS
- **Deployment**: GitHub Pages with CNAME configured for www.theios.org

## Key Files

- `index.html`: Main landing page with embedded styles and scripts
- `style.css`: Additional typography overrides (mostly redundant with inline styles)
- `style.min.css`: Minified version of external styles
- `CNAME`: Domain configuration for GitHub Pages (www.theios.org)
- Logo assets: `theios-logo-variant.png`, `theios-logo-favicon.png`, `favicon.png`

## Development Commands

This is a static site with no build process. Changes are made directly to HTML/CSS files.

For local development:
```bash
# Serve locally (requires Python 3)
python -m http.server 8000

# Or with Node.js
npx http-server
```

## Deployment

- Hosted on GitHub Pages
- Domain: www.theios.org (configured via CNAME)
- Auto-deploys from main branch
- SSL certificate managed by GitHub Pages

## External Links

The site contains links to:
- Theios Research Institute GitHub organization
- codex.nexus website (primary action button)
- Contact email: research@theios.org