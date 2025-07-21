# Cottage.js LangChain 插件

本插件用于在 Cottage.js 框架中集成 LangChain，实现 AI 对话能力。

## 快速开始

1. 安装依赖：
   ```bash
   npm install langchain @langchain/openai
   ```
2. 使用插件：
   ```js
   const langchainPlugin = require('../../src/plugins/langchainPlugin');
   const plugin = langchainPlugin({ apiKey: '你的OpenAI API Key' });
   plugin.chat([{ role: 'user', content: '你好' }]).then(console.log);
   ```

## 参数说明
- `apiKey`: OpenAI API 密钥
- `model`: 可选，默认 `gpt-3.5-turbo`

## 进阶用法

可结合 Cottage.js 的路由、组件等扩展更多 AI 场景。

---

详细文档见 [LangChain 官方文档](https://js.langchain.com/docs/)。
