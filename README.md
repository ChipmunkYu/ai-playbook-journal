# AI Workflow Playbook

这是一个长期持续更新的个人 AI 工作流与实践记录项目。

项目目标不是单纯展示 AI 生成结果、代码成果或课程作业，而是记录：

> 我如何在真实任务中与 AI 协作，以及这些协作方式如何演化。

它更接近 engineering / research journal、workflow notebook、field notes 与 AI collaboration playbook，而不是传统技术博客或单纯代码仓库。

## 项目关注什么

本仓库重点记录：

- AI workflow 的设计与变化
- Prompt 的使用、失败与优化
- Agent 协作方式
- AI 辅助研究与实验设计
- AI 辅助开发、调试与工程实践
- AI 图像生成中的风格、构图与约束控制
- AI 在学习、思考、实验中的参与方式
- 对 AI 行为的观察与反思

项目核心资产不是“AI 生成了什么”，而是：

- 如何逐步得到结果
- workflow 如何设计
- prompt 如何迭代
- AI 在哪里失败
- 如何约束模型
- 如何减少偏题
- 如何提高结果稳定性

## 当前理念

### 1. 低记录成本优先

项目仍处于大量探索阶段。不要为了严格分类、方法论命名、统一格式或高度结构化而提高记录门槛。

目标是让记录能够长期持续。

因此，本仓库允许：

- 碎片化记录
- 半成品内容
- 不成熟结论
- 只有观察而没有总结

### 2. 日志优先于方法论

当前阶段以 logs、experiments、raw observations 为主，不急于抽象 patterns、frameworks 或 methodologies。

方法论应当从长期记录中自然沉淀。

### 3. 保留真实探索痕迹

记录重点是过程、调整、失败、思考与观察，而不仅是最终成果。

本项目更重视真实探索痕迹，而不是“看起来完整”。

## 建议目录结构

```text
ai-workflow-playbook/
│
├── README.md
├── AGENTS.md
│
├── logs/
│   ├── 2026-05/
│   ├── 2026-06/
│   └── ...
│
├── prompts/
│   ├── image-generation/
│   ├── coding/
│   ├── research/
│   └── writing/
│
├── experiments/
│   ├── image-style-control/
│   ├── fairness-testing/
│   ├── agent-workflows/
│   └── ...
│
└── patterns/
```

### 目录说明

- `logs/`  
  当前最核心目录，用于低成本记录真实探索过程。

- `prompts/`  
  保存具有复用价值的 prompt、agent 配置与 workflow 模板。

- `experiments/`  
  放较完整的实验、测试与案例研究。

- `patterns/`  
  当前不是重点。只在长期积累后自然沉淀方法论。

## 记录风格

记录应更接近实验日志、工作随记与 field notes，而不是正式论文、教程或高度结构化知识库。

允许内容简短、未完成、不完整，甚至只有问题和观察。

优先保留：

- 当时的观察
- 调整过程
- AI 行为
- prompt 演化
- workflow 变化

## 当前重点主题

### AI 图像生成

包括中国古风 / 水墨风 prompt、构图控制、留白控制、风格漂移、局部修改、分阶段生成与 prompt refinement。

重点观察模型如何偏离约束，以及如何减少自由发挥、稳定风格。

### AI 辅助开发

包括 OpenCode、oh-my-opencode、agents、workflow orchestration、AI 调试、AI 辅助编译原理实验与 AI 辅助 web 开发。

重点观察 context 管理、agent 分工、prompt 结构，以及 AI 在复杂工程中的边界。

### AI 辅助科研

包括 fairness testing、semantic perturbation、paired testing、Δin / Δout、AI 辅助论文理解与 AI 辅助实验设计。

重点观察 AI 是否真正理解研究问题、AI 如何误导研究，以及如何避免“看似合理”的错误结论。

## AI 在本项目中的角色

AI 不只是内容生成器。

AI 可以参与：

- 记录辅助
- workflow 分析
- prompt 改进
- 思路整理
- 结构建议
- 方法论提炼
- 长期观察辅助

但 AI 不应：

- 过早抽象
- 强行总结
- 伪造规律
- 过度包装
- 把探索过程伪装成成熟理论

本仓库的长期目标，是从真实协作记录中逐步沉淀出可复用的 AI 工作流经验。
