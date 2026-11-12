<p align="center">
  <img src="tokeny.png" alt="Tokeny" width="112" height="112">
</p>

<h1 align="center">Tokeny</h1>

<p align="center">
  <strong>你的桌面 AI Agent 工作台</strong>
</p>

<p align="center">
  <a href="https://tokeny-ai.com">官网</a> ·
  <a href="https://space.bilibili.com/385462682">B站主页</a> ·
  <a href="https://github.com/tokeny-ai/tokeny/releases">下载</a> ·
  <a href="#界面预览">界面预览</a> ·
  <a href="#核心能力">核心能力</a> ·
  <a href="#系统要求">系统要求</a> ·
  <a href="#常见问题">常见问题</a>
</p>

<p align="center">
  <a href="https://github.com/tokeny-ai/tokeny/releases/tag/v1.8.1"><img src="https://img.shields.io/github/v/release/tokeny-ai/tokeny?display_name=tag&label=最新版本" alt="Latest release"></a>
  <a href="https://github.com/tokeny-ai/tokeny/releases"><img src="https://img.shields.io/github/downloads/tokeny-ai/tokeny/total?label=累计下载" alt="Downloads"></a>
  <a href="https://github.com/tokeny-ai/tokeny/releases/tag/v1.8.1"><img src="https://img.shields.io/badge/Windows-x64-0078D4" alt="Windows x64"></a>
</p>

---

Tokeny 是一个本地优先的桌面 AI 助手。它把多模型对话、Agent 工具调用、MCP 插件、Skills 技能、长期记忆、定时任务和 IM 集成放在同一个工作空间里，适合研究、写作、开发、运营和自动化任务。

数据默认保存在本机，模型请求只发送到你配置的 AI 服务商。你可以按工作空间管理文件、会话、权限、记忆和自动化流程。

## 最新版本

当前发布版本为 **v1.8.1**。本次 Release 已验证 Windows x64 安装包，并提供 SHA-256 校验文件。

## 下载

| 平台 | 当前下载 | 说明 |
| --- | --- | --- |
| Windows x64 | [Tokeny-1.8.1-windows-x64.exe](https://github.com/tokeny-ai/tokeny/releases/download/v1.8.1/Tokeny-1.8.1-windows-x64.exe) | NSIS 安装包，支持自定义安装目录 |
| 其他平台 | [查看全部 Releases](https://github.com/tokeny-ai/tokeny/releases) | 以对应 Release 页面提供的资产为准 |

Windows 安装包的 SHA-256：

```text
219D29F86EF2D0EC638D8D979745886D7B897D9AED0A0F3932AA2E58D1C8AF74
```

也可以下载 [Tokeny-1.8.1-windows-x64.exe.sha256](https://github.com/tokeny-ai/tokeny/releases/download/v1.8.1/Tokeny-1.8.1-windows-x64.exe.sha256) 后，在 PowerShell 中校验：

```powershell
Get-FileHash .\Tokeny-1.8.1-windows-x64.exe -Algorithm SHA256
```

安装后至少配置一个模型渠道即可开始使用。

## 界面预览

Tokeny 的主界面围绕工作空间组织。Agent 可以读取工作区文件、执行工具、生成内容，并在同一界面里沉淀会话和任务结果。

<table>
  <tr>
    <td align="center"><img src="screenshots/agent.png" alt="Agent 工作空间" width="420"><br><sub>Agent 工作空间</sub></td>
    <td align="center"><img src="screenshots/skills.png" alt="Skills 技能" width="420"><br><sub>Skills 技能</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/mcp.png" alt="MCP 插件" width="420"><br><sub>MCP 插件</sub></td>
    <td align="center"><img src="screenshots/plugin.png" alt="插件市场" width="420"><br><sub>插件市场</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/models.png" alt="模型配置" width="420"><br><sub>模型配置</sub></td>
    <td align="center"><img src="screenshots/memory.png" alt="记忆管理" width="420"><br><sub>记忆管理</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/schedule.png" alt="定时任务" width="420"><br><sub>定时任务</sub></td>
    <td align="center"><img src="screenshots/job.png" alt="执行结果" width="420"><br><sub>执行结果</sub></td>
  </tr>
  <tr>
    <td align="center"><img src="screenshots/im.png" alt="IM 集成" width="420"><br><sub>IM 集成</sub></td>
    <td align="center"><img src="screenshots/settings.png" alt="数据管理" width="420"><br><sub>数据管理</sub></td>
  </tr>
</table>

## 核心能力

- **多模型配置**：支持 OpenAI、Anthropic、DeepSeek、Google、MiniMax、硅基流动、火山方舟、Kimi、通义千问、智谱 GLM、小米 MiMo 以及兼容 OpenAI API 格式的服务。
- **Agent 执行环境**：基于工作空间运行，可读写文件、调用工具、拆解任务，并保留执行过程与结果。
- **MCP 插件系统**：通过 Model Context Protocol 扩展联网搜索、浏览器自动化、地图、笔记、企业协作和本地应用能力。
- **Skills 技能系统**：从技能市场安装或本地导入技能，为研究、代码、文档、表格、演示、视频、金融分析等场景提供专用能力。
- **长期记忆**：自动提取偏好、事实、指令和事件，支持全局记忆与工作空间记忆。
- **定时任务**：使用 Cron 表达式或固定周期运行 Agent 任务，支持手动触发和执行记录。
- **IM 集成**：连接飞书、微信等入口，让 AI 助手在消息流中回复和执行任务。
- **跨设备迁移**：导出和导入工作空间、会话、记忆、MCP、Skills 等数据，敏感信息可加密保护。
- **本地优先**：数据存储在本机 SQLite，日志和缓存可在设置中查看、清理和备份。

## 快速开始

1. 从 [Releases](https://github.com/tokeny-ai/tokeny/releases) 下载对应平台安装包。
2. 启动 Tokeny，进入设置中的 AI 模型配置。
3. 添加至少一个模型服务渠道，并选择默认对话模型。
4. 新建工作空间或打开已有项目目录。
5. 在输入框中直接对话，或通过 `/` 调用技能，通过 `@` 引用文件。

## 系统要求

- Windows 10 及以上，x64
- macOS 12 Monterey 及以上，arm64 或 x64
- 建议内存 8 GB 及以上
- 建议预留 500 MB 以上磁盘空间

## 常见问题

### Tokeny 会上传我的本地数据吗？

Tokeny 的工作空间、会话、记忆、日志和配置默认存储在本机。使用 AI 模型时，必要的提示词和上下文会发送给你配置的模型服务商；是否发送文件内容取决于你在会话中引用了哪些内容。

### 数据存储在哪里？

Windows 默认位于 `%APPDATA%/Tokeny`，macOS 默认位于 `~/Library/Application Support/Tokeny`。你也可以在设置的数据管理页查看存储概览、日志和迁移入口。

### 必须配置 API Key 吗？

需要。Tokeny 本身不内置模型服务，你需要配置至少一个 AI 服务商的 API Key 或兼容 OpenAI API 的 Base URL。

### 这是开源仓库吗？

当前仓库用于发布 Tokeny 安装包、截图和说明文档，不包含完整应用源码。

### 如何报告问题或提出建议？

可以在 [GitHub Issues](https://github.com/tokeny-ai/tokeny/issues) 提交问题，也可以通过 [官网](https://tokeny-ai.com) 或 [B站主页](https://space.bilibili.com/385462682) 了解最新动态。

---

<p align="center">
  Tokeny Team
</p>
