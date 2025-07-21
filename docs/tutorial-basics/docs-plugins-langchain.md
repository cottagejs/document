
---
sidebar_position: 8
title: LangChain 插件集成
---

# LangChain 插件集成

Cottage.js 支持通过插件集成 [LangChain](https://js.langchain.com/)，用于构建 AI 对话和智能应用。

## 安装依赖

```bash
npm install langchain @langchain/openai
```

## 插件用法

在 `src/plugins/langchainPlugin.js` 中：

```js
const langchainPlugin = require('./langchainPlugin');
const plugin = langchainPlugin({ apiKey: '你的OpenAI API Key' });

async function runChat() {
  const reply = await plugin.chat([
    { role: 'user', content: '你好，LangChain！' }
  ]);
  console.log(reply);
}
runChat();
```

## 配置说明
- `apiKey`: OpenAI API 密钥
- `model`: 可选，默认 `gpt-3.5-turbo`

## 集成到 Cottage.js

将插件注册到你的 Cottage.js 应用即可在任意组件或命令中调用。

---

更多 LangChain 用法请参考 [LangChain 官方文档](https://js.langchain.com/docs/)。
