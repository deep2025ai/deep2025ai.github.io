# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal academic CV website for Deep Shikha Srivastava (Materials Scientist, Entrepreneur, Educator). Built with Jekyll and hosted on GitHub Pages at https://deep2025ai.github.io/

## Build Commands

```bash
# Install dependencies
bundle install

# Run local development server
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

The site auto-deploys via GitHub Pages when pushing to the `main` branch.

## Architecture

**Single-page Jekyll site** with all content in `index.html`. Uses Liquid templating.

### Key Files
- `index.html` - All page sections (Hero, About, Research, Publications, Teaching, AeroGraphiX, CV)
- `_config.yml` - Site metadata and social links (LinkedIn, ORCID, email)
- `assets/css/style.css` - Complete design system with CSS variables for colors, typography, spacing
- `_layouts/default.html` - Base HTML template with CDN links for fonts/icons
- `_includes/nav.html` - Floating dot navigation component
- `_includes/footer.html` - Footer component

### Design System
CSS variables in `style.css` define the teal/green color palette (`--color-primary: #0d5c63`), typography (Inter font), and spacing tokens. Hexagonal SVG pattern inspired by graphene/h-BN research.

### Assets
- `assets/images/profile.jpg` - Profile photo
- `assets/files/Deep_Shikha_Srivastava_CV.pdf` - Downloadable CV
- `Resources/` - Source files (excluded from build)

### External Dependencies (via CDN)
- Google Fonts (Inter)
- Academicons (ORCID icon)
- Font Awesome (social/UI icons)
