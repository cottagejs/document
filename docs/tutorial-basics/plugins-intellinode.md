# Cottage.js IntelliNode 插件

本插件用于在 Cottage.js 框架中集成 IntelliNode，实现高效 Node.js API 服务。

## 快速开始

1. 安装依赖：
   ```bash
   npm install intellinode
   ```
2. 使用插件：
   ```js
   const intellinodePlugin = require('../../src/plugins/intellinodePlugin');
   const plugin = intellinodePlugin({
     routes: [
       {
         method: 'get',
         path: '/api/ping',
         handler: (req, res) => res.send('pong')
       }
     ]
   });
   plugin.listen(3000);
   ```

## 参数说明
- `routes`: 路由数组，包含 method、path、handler

## 进阶用法

可结合 Cottage.js 的路由、组件等扩展更多 API 场景。

---

详细文档见 [IntelliNode 官方文档](https://intellinode.dev/docs)。
