# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目定位

这是一个**个人持续学习笔记仓库**(README 标语:持续学习,不设限)。用于沉淀学习过程中的笔记、心得与示例代码,不是可交付的软件项目。

## 当前状态

- 仓库目前**几乎为空**:仅包含 `README.md`,尚无任何代码或笔记内容
- 尚无构建 / 测试 / 静态检查工具链(无 package.json、无配置文件、无 CI)
- 尚无 `.cursor`、`.ai-rules`、copilot 等 AI 辅助配置

因此当前没有可执行的 build / lint / test 命令。未来若引入内容或工具链,再补充本节。

## 约定

- 笔记建议按主题分目录存放,避免全部堆在根目录
- 添加可运行的代码示例时,请保持简洁自包含,便于单独执行验证
- 涉及 git 提交 / 分支合并 / 发版时,遵循用户全局 CLAUDE.md 中定义的流程(commit-push-pr、merge-to-test 等),当前仅有 `main` 分支
