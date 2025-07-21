---
sidebar_position: 2
title: Quick Start
---

# Quick Start

## Installation & Usage

1. Install dependencies
   ```sh
   npm install
   ```
2. Start development server
   ```sh
   npm run dev
   # or npx cottage dev
   ```
3. Build static site
   ```sh
   npm run build
   # or npx cottage build
   ```

## Directory Structure
- `cottage.config.js`: Main configuration file
- `server.js`: Node.js server entry
- `vite.config.js`: Vite build configuration
- `src/app.js`: Application main entry
- `src/components/`: Custom components directory
- `src/pages/`: Pages directory, supports content-driven rendering
- `src/content/`: Content resources (e.g. Markdown/MDX)
