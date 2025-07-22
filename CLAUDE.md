# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a minimalist static website hosted on GitHub Pages for Credentum (credentum.ai). The site displays a simple landing page with the tagline "Truth, remembered - especially when it wounds."

## Architecture & Structure

```
/
├── index.html         # Main HTML page with tagline display
├── CNAME             # GitHub Pages custom domain configuration (credentum.ai)
└── css/
    ├── reset.css     # CSS reset for cross-browser consistency
    ├── styles.css    # Main styles with responsive design
    └── themes/
        └── grey-white.css  # Color theme definitions
```

## Key Technical Details

- **Pure static site** - No build process, frameworks, or JavaScript
- **Responsive design** - Font sizes scale with viewport width using `vw` units
- **Font setup** - Uses Google Fonts (Roboto) with Font Awesome 5.12.0 loaded but unused
- **Color scheme** - Dark grey background (#485564) with white text (#FAFAFA)

## Development

Since this is a static site, development is straightforward:
- Edit HTML/CSS files directly
- View changes by opening `index.html` in a browser
- No build or compilation steps required
- Commits to main branch auto-deploy via GitHub Pages

## Deployment

The site automatically deploys to credentum.ai through GitHub Pages when changes are pushed to the main branch.