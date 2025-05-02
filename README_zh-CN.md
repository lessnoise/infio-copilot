<h1 align="center">Obsidian-Infio-Copilot</h1>

## 让你的 Obsidian 秒变个人 AI 工作站！

**Infio Copilot 是一款可高度个人定制化的 Obsidian AI 插件，旨在帮助用户在本地工作流中轻松使用各类强大的 AI 大模型，为知识库提供交互式对话、内联编辑、智能补全、全库检索问答等功能。**

[English Version](README.md)

[Chat with me on Twitter](https://x.com/buyiyouxi)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/felixduan)

## 🚀 为什么推荐 Infio Copilot？

- **本地优先**：秉承 Obsidian 相同的 local first 理念，让一切发生在本地
- **全面增强**：从段落、全篇改写到全库问答，覆盖知识库管理全流程
- **高度定制**：自由切换 LLM、配置提示模板，并可按需创建/切换专属 Agent 角色
- **极速响应**：向量数据通过本地数据库存储，使整体响应速度提升 2–3 倍
- **用户驱动**：我们是个人开发者、 Obsidian 深度用户，功能迭代源于真实痛点与社区反馈

## 最新版本

[0.2.4](https://github.com/infiolab/infio-copilot/releases/tag/0.2.4) 增加了多语言支持

[0.2.3](https://github.com/infiolab/infio-copilot/releases/tag/0.2.3) 增加了自定义模式配置，现在无法创建自己的 agent

[0.1.7](https://github.com/infiolab/infio-copilot/releases/tag/0.1.7) 增加了图片选择器模态框，允许用户在 Obsidian vault 或本地文件浏览器中搜索、选择和上传图片

[0.1.6](https://github.com/infiolab/infio-copilot/releases/tag/0.1.6) 更新了应用视图 (apply view)，现在可以在应用视图中编辑内容

## 核心特色功能

| 功能           | 描述                                                                  |
| -------------- | --------------------------------------------------------------------- |
| 🖋️ 内联编辑    | 选中文本 → 直接与 AI 讨论 → 一键应用到原段落                                   |
| 💬 对话式改写  | 与单个笔记进行智能对话，轻松修改或重写原文内容                                     |
| 📝 智能自动补全 | 边写边补，结合全局上下文，实时生成精准续写                                      |
| 🖼️ 图片识别    | 支持 Vault 内或本地图片上传 → AI 智能识别并分析（v0.1.7+）                     |
| 🔍 全库问答 (RAG)| 针对整个 Vault 提问，跨笔记检索并整合答案                                     |
| 🌐 DeepResearch| 根据问题搜索互联网数据，生成研究报告（轻量级）                                  |

### 🖋️ 内联编辑

选中文本 → 直接与 AI 讨论 → 一键应用到原段落

![inline-edit](asserts/edit-inline.gif)



### 💬 **对话式改写**

与单个笔记进行智能对话，轻松修改或重写原文内容
![chat-with-select](asserts/chat-with-select.gif)


### 📝 **智能自动补全**

输入时获取上下文感知的写作建议 （ ⬇️ 以下第4条为 AI 自动补全 ）

![autocomplte](asserts/autocomplete.gif)



🔍 **全库问答 (RAG)**

针对整个 Vault 提问，跨笔记检索并整合答案

![rag](asserts/rag.gif)

🖼️ **图片识别**

支持 Vault 内或本地图片上传→AI 智能识别并分析（v0.1.7+）




## 开始使用

> **⚠️ 重要提示：安装程序版本要求**
> Infio-Copilot 需要较新版本的 Obsidian 安装程序。如果您遇到插件无法正常加载的问题：
>
> 1. 首先，尝试在 `设置 > 通用 > 检查更新` 中正常更新 Obsidian。
> 2. 如果问题仍然存在，手动更新您的 Obsidian 安装程序：
>
>    - 从 [Obsidian 下载页面](https://obsidian.md/download) 下载最新安装程序
>    - 完全关闭 Obsidian
>    - 运行新的安装程序

1. 打开 Obsidian 设置
2. 导航至"社区插件"并点击"浏览"
3. 搜索 "Infio Copilot" 并点击安装
4. 在社区插件中启用该插件
5. 在插件设置中配置您的 API 密钥
   - SiliconFlow : [SiliconFlow API Keys](https://cloud.siliconflow.cn/account/ak)
   - OpenRouter : [OpenRouter API Keys](https://openrouter.ai/settings/keys)
	 - Alibaba Bailian : [Bailian API Keys](https://help.aliyun.com/zh/dashscope/developer-reference/activate-dashscope-and-create-an-api-key)
   - DeepSeek：[DeepSeek API Keys](https://platform.deepseek.com/api_keys/)
   - OpenAI：[ChatGPT API Keys](https://platform.openai.com/api-keys)
   - Anthropic：[Claude API Keys](https://console.anthropic.com/settings/keys)
   - Gemini：[Gemini API Keys](https://aistudio.google.com/apikey)
   - Groq：[Groq API Keys](https://console.groq.com/keys)
6. 设置快捷键以快速访问：
   - 转到 设置 > 快捷键
   - 搜索 "Infio Copilot"
   - 推荐的快捷键绑定：
     * Infio Copilot: Infio add selection to chat -> cmd + shift + L
     * Infio Copilot: Infio Inline Edit -> cmd + shift + K
![autocomplte](asserts/doc-set-hotkey.png)
7. 如果需要 跟文档聊天 , 需要配置 embedding 模型
	 - 目前之后 SiliconFlow Alibaba Google OpenAI 平台支持嵌入模型

## 反馈与支持
我们重视您的意见，并希望确保您能轻松分享想法和报告问题：

- **错误报告**：如果您遇到任何错误或意外行为，请在我们的 [GitHub Issues](https://github.com/infiolab/infio-copilot/issues) 页面提交问题。请确保包含尽可能多的细节，以帮助我们重现和解决问题。
- **功能请求**：对于新功能想法或改进建议，请使用我们的 [GitHub Discussions - Ideas & Feature Requests](https://github.com/infiolab/infio-copilot/discussions/categories/ideas) 页面。创建新的讨论来分享您的建议。

## 交流

![weixin](https://github.com/user-attachments/assets/bc985cee-b019-417d-b726-95c79b0043e4)


## 致谢

本项目站在巨人的肩膀上。我们要向以下开源项目表示感谢：

- [obsidian-copilot-auto-completion](https://github.com/j0rd1smit/obsidian-copilot-auto-completion) - 提供自动补全实现和 TypeScript 架构灵感
- [obsidian-smart-composer](https://github.com/glowingjade/obsidian-smart-composer) - 提供聊天/应用 UI 模式和 PgLite 集成示例
- [continue](https://github.com/continuedev/continue) & [cline](https://github.com/cline/cline) - 提供提示工程和 LLM 交互模式
- [pglite](https://github.com/electric-sql/pglite) - 提供对话/向量数据存储和示例代码

## 许可证

本项目采用 [MIT 许可证](LICENSE) 授权。
