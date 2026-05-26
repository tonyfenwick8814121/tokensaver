# 常见问题

## TokenSaver 是云服务吗？

不是。TokenSaver 在本地运行，只在授权、更新检查和问题反馈时访问 ClawNexus 服务。

## 会上传我的 OpenClaw 文件吗？

不会。TokenSaver 不上传 OpenClaw 文件、记忆文件、skills、提示词或用户文档。

## 标准版和专家版有什么区别？

标准版聚焦一键省 Token、Memory-Wiki 检测、Bootstrap 文档瘦身、上下文膨胀监控和本地备份恢复。

专家版增加能力地图、任务路由、Skill 分类标签、模型策略、调用规则和路由健康度测试。测试期内专家版能力免费开放。

## 为什么需要 Node.js？

当前 MCP 测试版基于 Node.js 运行。后续 Mac App 版本会尽量降低普通用户的安装门槛。

## 如何升级 TokenSaver？

启动时如发现新版本，控制台顶部会提示版本号并提供下载链接。下载新版并覆盖旧的程序文件即可；授权缓存、备份记录和 OpenClaw 工作区改动保存在程序包之外，不会因为覆盖安装而丢失。

## 如果我想重新测试，应该怎么做？

先在 TokenSaver 中执行恢复，确认 OpenClaw 已恢复到优化前状态；再删除 TokenSaver 本地状态。详细步骤见 [UNINSTALL.md](./UNINSTALL.md)。
