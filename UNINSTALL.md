# 恢复、卸载与重新测试

如果你想把本机 TokenSaver 恢复到“第一次安装前”的状态，建议按下面顺序操作。

## 1. 先恢复 OpenClaw

如果你已经运行过一键省 Token，请先打开 TokenSaver，进入备份与恢复，执行一键恢复。

不要先删除 TokenSaver 数据。备份记录通常保存在 OpenClaw 工作区的：

```text
.clawnexus-token-saver/backups
```

确认恢复完成后，再继续清理 TokenSaver 本地状态。

## 2. 删除 TokenSaver 本地授权和设置

macOS 默认位置：

```bash
rm -rf "$HOME/Library/Application Support/ClawNexus TokenSaver"
```

如果你曾经用过非 macOS 默认路径，也可以检查：

```bash
rm -rf "$HOME/.clawnexus-token-saver"
```

## 3. 删除旧的测试包

删除你解压出来的旧 TokenSaver 文件夹即可，例如：

```text
ClawNexus TokenSaver MCP Testing
```

## 4. 重新测试

重新下载最新版 zip，解压后双击：

```text
启动 TokenSaver.command
```

首次启动会重新生成匿名 install_id，并领取测试期授权。
