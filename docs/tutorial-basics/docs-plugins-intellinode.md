
---
sidebar_position: 9
title: IntelliNode 插件集成
---

# IntelliNode 插件集成

Cottage.js 支持通过插件集成 [IntelliNode](https://intellinode.dev/)，用于构建现代 Node.js API 服务。

## 安装依赖

```bash
npm install intellinode
```

## 插件用法

在 `src/plugins/intellinodePlugin.js` 中：

```js
const intellinodePlugin = require('./intellinodePlugin');
const plugin = intellinodePlugin({
  routes: [
    {
      method: 'get',
      path: '/api/hello',
      handler: (req, res) => res.json({ message: 'Hello from IntelliNode!' })
    }
  ]
});

plugin.listen(3000, () => {
  console.log('IntelliNode API server running on http://localhost:3000');
});
```

## 配置说明
- `routes`: 路由数组，包含 method、path、handler

## 集成到 Cottage.js

将插件注册到你的 Cottage.js 应用即可在任意组件或命令中调用。

---

更多 IntelliNode 用法请参考 [IntelliNode 官方文档](https://intellinode.dev/docs)。
