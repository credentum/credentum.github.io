# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a minimalist static website hosted on GitHub Pages for Credentum (credentum.ai). The site displays a simple landing page with the tagline "Truth, remembered - especially when it wounds."

## Architecture & Structure

```
/
├── index.html         # Main HTML page with tagline display
├── CNAME             # GitHub Pages custom domain configuration (credentum.ai)
├── css/
│   ├── reset.css     # CSS reset for cross-browser consistency
│   ├── styles.css    # Main styles with responsive design
│   └── themes/
│       └── grey-white.css  # Color theme definitions
└── .github/
    └── ISSUE_TEMPLATE/
        ├── investigation.md    # Template for unclear scope issues
        └── sprint-task.md      # Template for Claude Code ready tasks
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

## Issue Management

This repository uses GitHub Issue Templates to structure work:

### Investigation Template (`investigation.md`)
Use for problems with unclear scope that require systematic investigation:
- Documents symptoms without assumptions
- Tracks investigation progress and findings
- Captures root cause analysis and lessons learned
- Helps identify when to split complex issues

### Sprint Task Template (`sprint-task.md`)
Use for well-defined tasks ready for Claude Code execution:
- Includes Claude Code readiness checklist
- Estimates file scope (should be < 4 files, < 400 LoC)
- Contains pre-execution context and implementation notes
- Designed to be updated during AI-assisted implementation

When creating issues, choose the appropriate template based on whether the scope is clear and the task is ready for implementation.