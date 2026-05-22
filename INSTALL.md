# 安装说明

## macOS

1. 安装 Node.js 22.19 或更高版本。
2. 从 [Releases](https://github.com/tonyfenwick8814121/tokensaver/releases) 下载 `ClawNexus-TokenSaver-MCP-0.1.0-testing.zip`。
3. 解压。
4. 双击 `启动 TokenSaver.command`。

如果 macOS 阻止打开，请右键文件并选择“打开”。

## MCP 使用方式

用于 stdio MCP Host：

```bash
node "TokenSaverRuntime/dist/index.js" mcp
```

也可以直接运行包内的 `启动 MCP Server.command`。

## 版本建议

- Node.js：22.19+
- OpenClaw：建议 2026.5.12 到 2026.5.18
- macOS：Apple Silicon 和 Intel Mac 均可测试
