

---
sidebar_position: 3
title: Usage
---

# Usage

## Quick Start
Refer to `quickstart.md` for installation and basic usage.

## Directory Structure
- `src/pages/`: Page files (.js/.astro), auto route mapping
- `src/components/`: Client components (.jsx/.tsx), auto-bundled by Vite
- `src/content/`: Content resources (Markdown/MDX), for content-driven pages
- `src/plugins/`: Plugin extension directory, supports lifecycle hooks
- `docum/`: Project documentation

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
See other docs in `docum/` and the official README for advanced usage, plugin development, and deployment.

## 热重载与缓存优化
- 开发服务器自动监听页面变更，WebSocket 推送刷新
- Vite 构建与依赖缓存目录：`node_modules/.vite_cache`

## 自动化部署
- 可集成 Vercel/Netlify 等平台插件，详见 `vite.config.js` 注释

## 错误处理
- 页面渲染、路由、服务端异常均有详细错误提示
- 支持自定义 404/500 页面

---
如需更多示例与扩展，请参考 `src/plugins/pluginTemplate.js` 或补充文档！
