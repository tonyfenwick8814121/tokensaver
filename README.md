# ClawNexus TokenSaver

面向 OpenClaw 用户的本地词元节约工具。

TokenSaver 会先检查本机 OpenClaw 环境，再通过一键省 Token、能力地图和任务路由，减少每次对话里不必要的上下文注入。当前版本处于测试期，专家版能力免费开放测试。

## 下载

请到 [Releases](https://github.com/tonyfenwick8814121/tokensaver/releases) 下载最新版。

当前测试包：

- ClawNexus-TokenSaver-MCP-2026.6.10-testing.2.zip
- SHA256：`f15de17e495195720c52169ff069cc49c7ca1ab23f95afa31e7acb3e39da7936`

## 当前状态

- 版本：2026.6.10-testing.2
- 阶段：测试期
- 授权：测试期内默认开放专家版能力
- 发行包校验：Release 页面提供 SHA256
- 数据边界：本地运行，不上传 OpenClaw 文件、skills 或用户文档
- 更新方式：启动时自动检查新版，提示下载链接后由用户覆盖安装

## 版本更新

| TokenSaver 版本 | 兼容 OpenClaw 版本 |
| --- | --- |
| 2026.6.10-testing.2 | 2026.5.12 - 2026.6.10；修复一键恢复时启用后新增内容没有完整增量归档的问题 |
| 2026.6.10-testing.1 | 2026.5.12 - 2026.6.10；更新 OpenClaw 兼容范围至 2026.6.10 |
| 2026.6.5-testing.1 | 2026.5.12 - 2026.6.5；更新 OpenClaw 兼容范围至 2026.6.5 |
| 2026.6.1-testing.1 | 2026.5.12 - 2026.6.1；更新 OpenClaw 兼容范围至 2026.6.1 |
| 2026.5.28-testing.1 | 2026.5.12 - 2026.5.28；更新 OpenClaw 兼容范围至 2026.5.28 |
| 2026.5.26-testing.3 | 2026.5.12 - 2026.5.26；修复上下文膨胀瘦身后没有立刻归档进Wiki的问题 |
| 2026.5.22-testing.1 | 2026.5.12 - 2026.5.22 |
| 2026.5.22-testing | 2026.5.12 - 2026.5.22 |
| 2026.5.20-testing | 2026.5.12 - 2026.5.20 |

## 适合谁

- 正在使用 OpenClaw，并且明显感觉每轮对话 token 消耗偏高
- 安装了较多 skills，希望只在需要时加载相关能力
- 希望保留 OpenClaw 的使用方式，但减少重复上下文成本
- 愿意在测试期反馈真实问题，帮助 TokenSaver 变得更稳定

## 核心功能

### 标准版

- 一键省 Token：扫描 OpenClaw 上下文结构，给出可执行的优化方案
- Memory-Wiki 检测：确认归档能力是否可用，避免盲目瘦身
- Bootstrap 文档瘦身：在可恢复的前提下减少固定注入文档的冗余内容
- 上下文膨胀监控：持续观察核心文档是否再次变大
- 本地备份与恢复：高风险修改前自动备份，支持一键恢复
- Memory Search 检测：发现记忆搜索不可用、embedding 配置异常等问题

### 专家版（免费测试中）

- 能力地图：整理本机 skills，形成可查询、可维护的能力索引
- 任务路由：根据对话任务选择需要注入的 skills，而不是全量注入
- Skill 分类与标签：支持按能力域、输入对象、输出形态、触发线索等维度整理
- 模型策略：按任务类型选择默认模型和回退模型
- 调用规则：支持域名、关键词、链接等场景下的指定 skill 调用
- 路由健康度测试：检查失效 skill、规则冲突和模型策略缺口

## 安全与隐私

TokenSaver 默认在本地运行，不上传你的 OpenClaw 文件、记忆文件、skills、提示词或用户文档。

会访问 ClawNexus 服务的场景仅包括：

- 测试期授权
- 更新检查
- 问题反馈

测试期授权使用本机生成的匿名 `install_id`，不上传原始 MAC 地址。

## 运行要求

- macOS，支持 Apple Silicon 和 Intel Mac
- Node.js 22.19 或更高版本
- 建议 OpenClaw 版本：2026.5.12 到 2026.6.10

## 快速开始

1. 从 [Releases](https://github.com/tonyfenwick8814121/tokensaver/releases) 下载 zip 包。
2. 解压。
3. 双击 `启动 TokenSaver.command` 打开本地控制台。
4. 如果需要作为 MCP Server 使用，运行 `启动 MCP Server.command`。首次运行会自动把 TokenSaver 注册到 OpenClaw 的 MCP 配置中，后续启动会先检查配置是否仍然正常。

如果 macOS 阻止打开，请右键文件并选择“打开”。

## 重新测试或卸载

如果你想完全重新测试，请先恢复 OpenClaw，再清理 TokenSaver 本地状态。详细步骤见 [UNINSTALL.md](./UNINSTALL.md)。

## 反馈

遇到问题时，优先使用 TokenSaver 内置的“问题与反馈”。也可以在本仓库提交 Issue。
