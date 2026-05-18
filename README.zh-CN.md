# Claude Agent SDK 示例合集

> ⚠️ **重要说明**：本仓库中的示例由 Anthropic 提供，仅用于本地开发学习，**请勿**部署到生产环境或在大规模场景下使用。

本仓库包含多个 [Claude Agent SDK](https://platform.claude.com/docs/en/agent-sdk/overview) 的演示项目，展示如何用 Claude 构建不同类型的 AI 应用。

**英文版说明请见 [README.md](./README.md)。**

## 可用示例

### 📧 [Email Agent](./email-agent)
开发中的 IMAP 邮件助手，支持：
- 展示收件箱
- 执行智能检索以查找邮件
- 提供由 AI 驱动的邮件辅助能力

### 📊 [Excel Demo](./excel-demo)
演示如何用 Claude 处理电子表格与 Excel 文件。

### 👋 [Hello World](./hello-world)
入门示例，帮助理解 Claude Agent SDK 的基本用法。

### 🔄 [Hello World V2](./hello-world-v2)
V2 Session API（`unstable_v2_*`）示例：使用独立的 `send()` / `stream()`，而非单一的 `query()` 生成器；包含多轮对话与会话持久化等用法。

### 🔬 [Research Agent](./research-agent)
多 Agent 研究系统：协调专职子 Agent 进行研究并生成综合性报告：
- 将研究需求拆分为子课题
- 并行启动检索型子 Agent 进行网络搜索
- 将结果整合为详尽报告
- 展示细致的子 Agent 活动追踪

### 🎨 [AskUserQuestion Previews](./ask-user-question-previews)
品牌类助手演示：将 AskUserQuestion 的选项渲染为可视化 HTML 预览卡片，而非纯文本标签：
- 启用 `previewFormat: "html"`，使每个选项包含带样式的 HTML 示意
- 通过 WebSocket，在 SDK 的 `canUseTool` 回调与浏览器之间往返传递问题
- 演示如何通过计划模式，引导 Claude 在行动前先提出澄清性问题

### 💬 [Simple Chat App](./simple-chatapp)
基于 SDK 的 React + Express 聊天界面，通过 WebSocket 展示完整对话循环与流式响应。

### 📄 [Resume Generator](./resume-generator)
根据对人名进行的网络检索（LinkedIn、GitHub、新闻等）汇总信息，生成一页 `.docx` 简历。

## 快速开始

每个示例自有独立目录与安装说明。请进入对应子目录，并遵循该目录中的 README 完成配置与运行。

## 环境要求

- [Bun](https://bun.sh) 运行时（或使用 Node.js 18+）
- Anthropic API 密钥（[在此获取](https://console.anthropic.com)）

## 上手步骤

1. **克隆本仓库**

```bash
git clone https://github.com/anthropics/claude-agent-sdk-demos.git
cd claude-agent-sdk-demos
```

2. **选择示例并进入其目录**

```bash
cd email-agent  # 或 excel-demo、hello-world 等
```

3. **阅读该示例自带的 README**，按说明完成安装与使用

## 相关资源

- [Claude Agent SDK 文档](https://platform.claude.com/docs/en/agent-sdk)
- [API 参考](https://platform.claude.com/docs/en/agent-sdk/api-reference)
- [GitHub Issues](https://github.com/anthropics/claude-agent-sdk-demos/issues)

## 支持与反馈

这些示例按「现状」提供。若遇到问题，可按类型查阅：

- **Claude Agent SDK 本身**：[SDK 文档](https://platform.claude.com/docs/en/agent-sdk)
- **本仓库示例相关**：[GitHub Issues](https://github.com/anthropics/sdk-demos/issues)
- **API 使用问题**：[Anthropic 支持](https://support.anthropic.com)

## 许可

MIT — 示例代码仅供演示与学习使用。
