# ClawNexus TokenSaver

ClawNexus TokenSaver is a local token-saving tool for OpenClaw users. The current release is a testing build, and Expert features are available during the testing period.

## Download

Download the latest package from the GitHub Releases page.

Current testing package:

- ClawNexus-TokenSaver-MCP-0.1.0-testing.zip
- SHA256: `f31d2e3da8d7431106ba11a130387fa9a8aaef24511059346f26a98aa4cb2042`

## What it does

- Checks the local OpenClaw environment
- Helps reduce unnecessary context loaded into conversations
- Provides a local MCP server for advanced OpenClaw workflows
- Offers Memory Search checks and guided repair
- Keeps backups before risky local changes

## Requirements

- macOS on Apple Silicon or Intel
- Node.js 22.19 or newer
- OpenClaw 2026.5.12 to 2026.5.18 is recommended

## Quick start

1. Download the zip package from Releases.
2. Unzip it.
3. Double-click `启动 TokenSaver.command` to open the local console.
4. Use `启动 MCP Server.command` when you want to mount TokenSaver as an MCP server.

## Privacy

TokenSaver runs locally. It does not upload your OpenClaw files, memory files, skills, prompts, or raw device identifiers. The app contacts ClawNexus services for testing-period authorization, update checks, and feedback submission.

## Feedback

Please submit issues through the TokenSaver feedback form or this repository's Issues page.

## 中文说明

ClawNexus TokenSaver 是面向 OpenClaw 用户的本地 token 节约工具。当前版本处于测试期，测试期内开放专家能力。

### 下载

请前往 GitHub Releases 下载最新版。

当前测试包：

- ClawNexus-TokenSaver-MCP-0.1.0-testing.zip
- SHA256: `f31d2e3da8d7431106ba11a130387fa9a8aaef24511059346f26a98aa4cb2042`

### 主要功能

- 检查本机 OpenClaw 环境
- 减少对话中不必要的上下文加载
- 提供本地 MCP Server
- 检测 Memory Search 状态，并提供引导式修复
- 在高风险本地修改前保留备份

### 运行要求

- Apple Silicon 或 Intel Mac
- Node.js 22.19 或更高版本
- 建议 OpenClaw 版本：2026.5.12 到 2026.5.18

### 使用方式

1. 从 Releases 下载 zip 包。
2. 解压。
3. 双击 `启动 TokenSaver.command` 打开本地控制台。
4. 如果需要挂载 MCP Server，运行 `启动 MCP Server.command`。

### 隐私

TokenSaver 在本地运行，不上传你的 OpenClaw 文件、记忆文件、skills、提示词或原始设备标识。软件会访问 ClawNexus 服务，用于测试期授权、更新检查和问题反馈。
