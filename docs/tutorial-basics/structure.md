

---
sidebar_position: 4
title: Directory Structure
---

# Directory Structure

## Main Directory Overview
- `src/pages/`: Page files (.js/.astro), auto route mapping
- `src/components/`: Client components (.jsx/.tsx), auto-bundled by Vite
- `src/content/`: Content resources (Markdown/MDX), for content-driven pages
- `src/plugins/`: Plugin extension directory, supports lifecycle hooks
- `docum/`: Project documentation

## Configuration Files
- `cottage.config.js`: Main config, includes plugins, build, directory settings
- `vite.config.js`: Vite build and production optimization config

## Development Mode
- Auto hot reload after editing pages/components/content
- Plugins can extend render, build, routing, etc.
- SSR/SSG dual mode, controlled by `BUILD_MODE` environment variable

## Extension Points
- Routing, rendering, build, hot reload, deployment, etc. can be extended via plugins

For more plugin development and advanced configuration, see "Plugin System & Extensions" and other docs in `docum/`.
