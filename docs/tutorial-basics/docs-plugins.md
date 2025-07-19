---
sidebar_position: 5
title: Plugins & Extensions
---

# Plugins & Extensions

## Plugin Registration
- Add plugin path or package name in the `plugins` array of `cottage.config.js`
- Plugins must export standard lifecycle hooks (see `src/plugins/pluginTemplate.js`)

## Lifecycle Hooks
- `beforeRender(ctx)`: Before page render
- `afterRender(ctx)`: After page render
- `notFound(ctx)`: When route not matched
- `buildStart(ctx)`: When static build starts
- `buildEnd(ctx)`: When static build ends
- `hotReload(ctx)`: Hot reload event

## Plugin Development Example
```js
module.exports = {
  beforeRender(ctx) {
    // You can modify ctx.html or log
  },
  afterRender(ctx) {
    // You can modify ctx.html or inject content
  },
  notFound(ctx) {
    // Custom 404 response
  },
  buildStart(ctx) {
    // Custom logic before static build starts
  },
  buildEnd(ctx) {
    // Custom logic after static build ends
  },
  hotReload(ctx) {
    // Custom logic on hot reload event
  }
};
```

## Extension Points
- Routing, rendering, build, hot reload, deployment, etc. can all be extended via plugins

For more advanced usage, see "Vite Configuration & Production Optimization" and other docs.
