# 更新日志

## 0.1.0-testing hotfix

- 增加 OpenClaw MCP 自动注册：首次运行 MCP Server 会写入 `tokensaver` MCP 配置，后续启动会自动检查并保持幂等。
- 适配并验证 OpenClaw 2026.5.20，建议版本范围更新到 2026.5.12 到 2026.5.20。
- 统一 MCP Web Console 的桌面工具视觉：侧栏、标题区、卡片、按钮、输入框和三栏工作台改为 TokenSaver 当前设计语言。
- 按测试期方案精简设置页，保留授权刷新、更新检查和反馈入口，不展示购买、续订或订阅详情页面。
- 调整任务路由默认页，优先展示“搜索 / 爬虫”，轻量问答等 0 skill 分类不再误塞无关技能。
- 补齐 Web Console 的能力地图页面：读取真实 Skills、分类、搜索筛选、详情编辑、标签/调用提示/启停保存。
- 补齐 Web Console 的任务路由页面：读取真实任务分类、模型选择、技能队列、调用规则、策略保存和路由测试。
- 增加能力地图与任务路由的 HTTP 接口测试，避免页面退化成入口占位。
- 补回 Web Console 的一键省 Token 页面入口。
- 增加优化预案、开启一键省 Token、备份列表和一键恢复入口。
- 修复总览页体检与 MCP Manifest 结果不明显的问题，输出区域会自动滚动到最新结果。

## 0.1.0-testing

- 发布 TokenSaver MCP 测试期版本。
- 接入 ClawNexus 测试期授权。
- 提供本地 Web Console 和 MCP Server。
- 增加一键省 Token、能力地图、任务路由相关入口。
- 增加 Memory Search 检测与引导式修复入口。
- 接入更新检查与问题反馈提交。
- 支持 Apple Silicon 和 Intel Mac。
- 建议 OpenClaw 版本：2026.5.12 到 2026.5.18。
