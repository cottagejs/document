---
sidebar_position: 2
title: Quick Start
---

# Quick Start

Cottage.js is a content-driven, component-based Node.js framework for modern web apps and content sites. It supports static and dynamic rendering, plugin extension, and configuration-driven development.

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
- `webpack.config.js`: Build configuration
- `src/app.js`: Application main entry
- `src/components/`: Custom components directory
- `src/pages/`: Pages directory, supports content-driven rendering
- `src/content/`: Content resources (e.g. Markdown/MDX)

## Common CLI Commands
- `cottage dev`: Start development server
- `cottage build`: Build static site
- `cottage clean`: Remove build output directory
- `cottage preview`: Preview static site from build output
- `cottage info`: Show project configuration and environment info
- `cottage list-pages`: List all available pages

## Plugin & Extension
- Register plugins in `cottage.config.js` under the `plugins` array
- Plugins must implement standard lifecycle hooks (see `src/plugins/pluginTemplate.js`)
- Extend routing, rendering, build, hot reload, deployment, etc. via plugins

For advanced configuration and usage, see the documentation in the `docum/` folder and the official README.


