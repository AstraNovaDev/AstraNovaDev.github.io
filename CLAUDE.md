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

- **CSS Custom Properties**: Comprehensive design system with color palette, typography scale, and spacing variables in `:root`
- **Color System**: 
  - Adaptive color scheme with automatic dark/light mode detection via `prefers-color-scheme`
  - BodyOS brand color: `#fc240f` (sunburst red-orange) with lighter/darker variants
  - Monochrome grayscale palette (50-900) for neutral elements
- **Responsive Design**: Mobile-first approach with breakpoint-based media queries
- **Layout Systems**: CSS Grid for product sections, Flexbox for navigation and footer layouts
- **Typography**: Inter font family with predefined size scale (xs to 5xl)

## JavaScript Features

The `index.html` includes sophisticated client-side functionality:

- **Google Analytics**: Integrated tracking with gtag
- **Scroll Animations**: Apple-style parallax effects for hero, product sections, and staggered reveals
- **Form Handling**: Dynamic waitlist form submission to Google Forms with loading states
- **DNA Animation**: Dynamically generated scrolling DNA sequences with opacity gradients
- **URL State Management**: Hash-based navigation for thank-you messages
- **Performance Optimizations**: Throttled scroll events using `requestAnimationFrame`

## Brand Assets Structure

- `assets/brand_assets/AstraNova/` - Company logo variations (black, white, horizontal)
- `assets/brand_assets/BodyOS/` - Product branding with icons and logos in multiple formats
- All assets provided in multiple sizes (1000px, 2000px) and formats (PNG)

## External Integrations

- **Google Forms**: Waitlist submission via hidden iframe method
- **External Links**: BodyOS web app (`bodyosapp.com`) for alpha access
- **GitHub Pages**: Automatic deployment from main branch to custom domain (`www.astranovallc.com`)