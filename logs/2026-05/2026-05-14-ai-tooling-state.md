# 2026-05-14 AI tooling state

当前主要使用：

- model：GPT 系列为主
- IDE：VSCode
- agent / runtime：OpenCode
- 配置增强：oh-my-opencode

初步观察：

- 这套组合更像是把 AI 接入到日常开发环境里，而不是单独开一个聊天窗口。
- OpenCode 让任务可以被拆成 agent / subagent 协作，但是否真的提升效率，取决于任务拆分和 context 管理。
- oh-my-opencode 降低了配置和 workflow 组织成本，但也可能让我更依赖预设的 agent 分工。
- 目前还不确定：实际效率提升主要来自 model 能力，还是来自 VSCode + OpenCode + oh-my-opencode 这套接入方式。

待继续观察：

- 长任务中，subagent 是否真的减少主上下文负担？
- GPT 在代码修改、日志整理、科研理解这几类任务里的边界是否不同？
- 工具链越复杂，是否会增加"看似自动化但实际需要人工协调"的成本？
- 哪些任务适合 agent 化，哪些任务反而直接对话更快？

备注：

这不是固定配置说明，只是当前阶段的使用状态记录。后续如果工具链、模型或使用方式变化，可以继续追加，而不是回头改写成完整方法论。

---

## 2026-05-29 更新：切换至 DeepSeek

### 变更

- 模型从 GPT 系列切换至 DeepSeek 系列
- 默认模型：`opencode-go/deepseek-v4-flash`（省钱方案）
- 深度分析模型：`opencode-go/deepseek-v4-pro`（通过 oracle agent）
- 订阅：OpenCode Go

### Agent 模型分配

| Agent | 模型 | 用途 |
|-------|------|------|
| orchestrator | deepseek-v4-flash | 日常编排 |
| oracle | deepseek-v4-pro | 深度分析 |
| council | deepseek-v4-pro | 多角度审查 |
| librarian | deepseek-v4-flash | 文档查询 |
| explorer | deepseek-v4-flash | 代码搜索 |
| designer | deepseek-v4-flash | UI 设计 |
| fixer | deepseek-v4-flash | 执行任务 |

### 切换原因

- GPT 系列成本较高，DeepSeek 在编码和工具调用方面性价比更好
- flash 模型足够处理日常编排任务，pro 模型在需要深度思考时按需调用
- OpenCode Go 订阅提供了稳定的 DeepSeek 模型访问

### 作者标注规范

从本次更新起，AI 生成的分析文件需在开头标注模型信息：

- 默认分析：`AI（opencode-go/deepseek-v4-flash）`
- 深度分析：`AI（opencode-go/deepseek-v4-pro）`
- 历史文件（2026-05-29 前）：`AI（openai/gpt-5.5）`
