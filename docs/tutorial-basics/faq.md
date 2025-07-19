---
sidebar_position: 7
title: FAQ
---

# FAQ

## What is Cottage.js?
Cottage.js is a content-driven, component-based Node.js framework for modern web apps and content sites. It supports static and dynamic rendering, plugin extension, and configuration-driven development.

## How do I install and start a project?
See `quickstart.md` for installation and usage instructions.

## How do I add a new page?
Add a `.js` or `.astro` file to the `src/pages/` directory. The framework will automatically map routes based on file structure.

## How do I create a custom component?
Add a `.jsx` or `.tsx` file to the `src/components/` directory. Components are auto-bundled by Vite.

## How do I register a plugin?
Add the plugin path or package name to the `plugins` array in `cottage.config.js`. Plugins must implement lifecycle hooks.

## How do I switch between SSR and SSG?
Set the environment variable `BUILD_MODE=ssr` or `BUILD_MODE=ssg` before building.

## Where can I find more documentation?
See all docs in the `docum/` folder and the official README for advanced usage, plugin development, and deployment.

## How do I get help or contribute?
Open issues or discussions on GitHub. Contributions and feedback are welcome!
