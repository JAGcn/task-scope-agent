# Codex 任务边界整合包

用 `task-scope` 交办任务。Skill 区分用户要求和附件材料，把标准案件包交给独立的 `task_scope_judge` 裁定。实施事项确认就绪后，主助手按已确认的范围执行并验证。

## 下载与安装

下载 [task-scope-agent.zip](task-scope-agent.zip) 并解压。整合包内的 `README.md` 提供完整安装说明、使用示例和裁定协议。

1. 将解压出的 `task-scope/` 目录放到 `~/.codex/skills/`。
2. 将解压出的 `.codex/agents/task_scope_judge.toml` 放到 `~/.codex/agents/`。
3. 如需全局使用三条端到端指标规则，将 `docs/codex-instructions.md` 的内容合并到「设置 → 个性化 → Codex 指令」。
4. 新建 Codex 对话加载配置。已有一条明确的待处理任务时，发送 `task-scope` 即可。

### 追加事项测速

> task-scope，审查这条追加要求，并记录端到端指标。

端到端指标包括从提出到可执行结论的总耗时、每项人工确认轮数和实际越界返工次数及成本。解压后可在 `task-scope/references/metrics.md` 查看统计口径，在 `docs/任务边界整合包报告.docx` 查看中文说明。

### 文件校验

`task-scope-agent.zip` 的 SHA-256 为 `00c219100ba0ac1e61fd5eabecfcd5dcf505092ec7ae9db0f147a9d9628de16a`。
