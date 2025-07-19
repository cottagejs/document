---
sidebar_position: 6
title: Vite & Production
---

# Vite Configuration & Production Optimization

## Advanced Configuration
- Supports alias, CSS preprocessors, environment variables, plugin registration
- SSR/SSG dual mode, switch with `BUILD_MODE=ssr` or `BUILD_MODE=ssg`
- Output directory automatically separated (dist-ssr/dist)
- Register Vite plugins in `vite.config.js`

## Cache Optimization
- Build and dependency cache directory: `node_modules/.vite_cache`
- Dev server supports file system cache for faster reloads

## Automated Deployment
- Integrate platform plugins like Vercel/Netlify for CI/CD
- Configure deploy parameters in `vite.config.js`

## Production Recommendations
- Enable minification and code splitting to improve load speed
- Configure assetsDir for better static asset management
- Use environment variables to separate dev/production logic
- Optimize SSR/SSG output for SEO and performance

For more details, see Vite official docs and Cottage.js plugin extensions.
