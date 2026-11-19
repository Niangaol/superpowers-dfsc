# superpowers-dfsc

[obra/superpowers](https://github.com/obra/superpowers) 的 DFSC / Step Code 打包副本，供 DFSC 社区市场 `dfsc-community` 收录分发。

- 上游项目：obra/superpowers（作者 Jesse Vincent，MIT）
- 上游版本：7.0.2
- 打包内容：`skills/`（15 个技能）、`LICENSE`、上游 `README.md`、`.claude-plugin/plugin.json`
- 未包含：各平台适配层（OpenCode / Codex / Cursor / Kimi / Hermes / Pi 等）、Claude Code 的 `hooks/`、维护脚本 `scripts/`、测试与设计文档、图片素材

插件资源位于 [plugins/superpowers](plugins/superpowers/)，安装后通过 `step.plugin.json` 的 `skills` 声明加载全部技能。

说明：

- 上游 `hooks/` 不在打包范围内（DFSC 无文件式 hooks），`using-superpowers` 的会话启动自动提示不会出现，技能需显式调用或由 AGENTS.md 指引。
- `brainstorming` 的可视化伴侣会在本机启动 node 进程并在 `127.0.0.1` 随机端口监听，仅在启用该功能时使用。
- 本仓库仅做格式适配与打包，不修改技能内容；问题与改进请先反馈上游。

License: MIT（见 [plugins/superpowers/LICENSE](plugins/superpowers/LICENSE)）

对应上游提交：`22f0b463e7a5e579904dd6211a520321035526f7`（打包时指向 obra/superpowers main 的最新提交）
