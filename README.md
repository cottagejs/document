# Website

This website is built using [Docusaurus](https://docusaurus.io/), a modern static website generator.

## Installation

```bash
yarn
```

## Local Development

```bash
yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

访问 http://localhost:3000 查看效果。

## Build

```bash
yarn build
```

This command generates static content into the `build` directory and can be served using any static contents hosting service.

## Deployment

Using SSH:

```bash
USE_SSH=true yarn deploy
```

Not using SSH:

```bash
GIT_USER=<Your GitHub username> yarn deploy
```

If you are using GitHub pages for hosting, this command is a convenient way to build the website and push to the `gh-pages` branch.

## Docusaurus 中文文档网站

本项目基于 Docusaurus 初始化，适合搭建中文文档和博客。

### 快速开始

1. 进入项目目录：
   ```powershell
   cd website
   ```
2. 启动开发服务器：
   ```powershell
   npm start
   ```

### 主要命令
- `npm start`：本地开发
- `npm run build`：打包生产环境
- `npm run serve`：本地预览打包结果
- `npm run deploy`：部署到 GitHub Pages

### 目录结构
- `docs/`：文档内容
- `blog/`：博客内容
- `src/`：自定义页面和组件

---
如需自定义为中文界面，请修改 `docusaurus.config.js` 的 `i18n` 配置。
