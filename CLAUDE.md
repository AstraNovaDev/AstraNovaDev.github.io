# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the company website for AstraNova LLC (`AstraNovaDev.github.io`), a static HTML/CSS site showcasing their health technology company and flagship product BodyOS. The site is hosted on GitHub Pages.

## Architecture

- **Static Site**: Single-page HTML website with vanilla CSS styling
- **No Build Process**: Direct HTML/CSS files served by GitHub Pages
- **Assets Structure**:
  - `assets/styles/main.css` - Main stylesheet with CSS custom properties
  - `assets/images/logo.svg` - Company logo
  - `assets/brand_assets/` - Brand assets including icons and logos in various formats
- **Deployment**: Automatic via GitHub Pages when pushed to main branch

## Key Files

- `index.html` - Main landing page with sections for hero, product (BodyOS), about, and contact
- `assets/styles/main.css` - Stylesheet using CSS custom properties for theming
- `CNAME` - Domain configuration for GitHub Pages
- `README.md` - Basic project identification

## Development Commands

Since this is a static site with no build process:

- **Local Development**: Open `index.html` directly in browser or use a local server
- **Testing**: Manual browser testing across different screen sizes
- **Deployment**: Push to main branch triggers automatic GitHub Pages deployment

## Site Structure

The single-page site includes:
- Header with navigation and hero section
- Product section showcasing BodyOS
- About section describing AstraNova LLC
- Contact form (mailto action)
- Footer with company details

## Styling Architecture

- CSS custom properties (CSS variables) defined in `:root`
- Mobile-first responsive design with media queries
- Dark theme with orange accent color (`#ff4f00`)
- Grid layout for product section
- Flexbox for navigation and footer