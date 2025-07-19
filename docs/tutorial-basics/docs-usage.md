---
sidebar_position: 3
title: Usage
---

# Usage

Refer to Quick Start for installation and basic usage.

## Development Mode
- Auto hot reload after editing pages/components/content
- Plugins can extend render, build, routing, etc.
- Supports SSR/SSG dual mode, controlled by `BUILD_MODE` environment variable

## SSR/SSG Dual Mode
- Set `BUILD_MODE=ssr` or `BUILD_MODE=ssg` to switch SSR/SSG build
- SSR output: `dist-ssr`, SSG output: `dist`

## Plugin System
- Register plugins in `cottage.config.js` under `plugins` array
- Plugins must implement lifecycle hooks (see `src/plugins/pluginTemplate.js`)

## Advanced Vite Configuration
- Supports alias, CSS preprocessors, minification, environment variables, automated deployment
- Register Vite plugins in `vite.config.js`

## More
See other docs and the official README for advanced usage, plugin development, and deployment.
