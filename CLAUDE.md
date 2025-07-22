# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a farewell landing page for Hummingbird Hammocks, a small business that specialized in ultralight camping and backpacking gear. The company closed after 10 years of operation. The site serves as a memorial and provides information about their open-source contributions.

## Technology Stack

- **HTML/CSS/JavaScript**: Static landing page
- **Tailwind CSS**: Utility-first CSS framework for styling
- **Flowbite**: UI component library built on Tailwind CSS
- **PostCSS**: CSS processing with autoprefixer and cssnano for minification
- **Node.js**: Development environment and build tools

## Common Development Commands

### Development
```bash
npm run dev
```
Runs Tailwind CSS in watch mode, compiling `input.css` to `output.css` with live reloading for development.

### Building for Production
```bash
npm run build
```
Complete production build that:
1. Compiles and minifies CSS (`npm run build:css`)
2. Minifies HTML (`npm run build:html`) 
3. Copies assets to dist directory (`npm run copy:assets`)

### Individual Build Steps
```bash
npm run build:css    # Compile CSS with PostCSS minification to dist/
npm run build:html   # Minify HTML to dist/index.html
npm run copy:assets  # Copy images and other assets to dist/
```

## Project Structure

- `index.html` - Main landing page with company farewell message and open-source repository links
- `input.css` - Source Tailwind CSS file
- `output.css` - Compiled CSS for development
- `dist/` - Production build output directory
- `images/` - Static assets (logos, product photos)
- `tailwind.config.js` - Tailwind configuration with Flowbite integration
- `postcss.config.js` - PostCSS configuration for production builds

## Key Features

The landing page includes:
- Company farewell message and closure explanation
- Statistics about their 10-year journey (customers served, gear sold, trees planted)
- Links to all open-source repositories (hammocks, tarps, accessories, etc.)
- FAQ section about recommendations and open-source usage
- Responsive design using Tailwind CSS utility classes

## Styling Notes

- Uses custom color palette with earth tones (`#fdfdf6`, `#34542a`, `#0f220e`, `#f3f3ec`)
- Extensive use of Tailwind utility classes for responsive design
- Flowbite components for interactive elements (accordion FAQ section)
- All external resources (Flowbite CSS/JS) are included locally