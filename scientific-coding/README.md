# 科学 Coding 观

`scientific-coding` 是一个面向 AI 编程 Agent 的公开 Skill。

它适用于 Codex、Claude Code、Cursor、Cline、GitHub Copilot 等 AI Coding Agent，用来约束 Agent 在真实工程项目中的行为：先读上下文，再写代码；先确认事实，再调用接口；先验证结果，再宣布完成。

## 核心理念

AI 编程 Agent 的价值不是替代程序员思考，而是提升工程效率。

优秀的 Agent 不应该：

- 凭空猜测；
- 随意修改；
- 编造实现；
- 忽略上下文；
- 跳过验证。

而应该：

- 基于事实；
- 理解上下文；
- 遵循规范；
- 主动验证；
- 谨慎修改；
- 诚实表达不确定。

一句话：

> 少一点幻想，多一点查询；少一点猜测，多一点确认；少一点生成，多一点验证。

## 目录结构

```text
scientific-coding/
├── SKILL.md
├── README.md
├── RULES.md
├── CHECKLIST.md
├── PROMPTS.md
├── agents/
│   └── openai.yaml
├── examples/
│   ├── correct_workflow.md
│   └── hallucination_cases.md
└── templates/
    └── task_report.md
```

## 文件说明

- `SKILL.md`：Skill 入口文件，Agent 主要读取它。
- `RULES.md`：完整“科学 Coding 观”和十六荣十六耻。
- `CHECKLIST.md`：开发前、开发中、开发后的检查清单。
- `PROMPTS.md`：可直接复制使用的提示词模板。
- `examples/`：正确流程和错误案例。
- `templates/task_report.md`：任务完成报告模板。
- `agents/openai.yaml`：Skill UI 元数据。

## 使用方式

把整个 `scientific-coding/` 文件夹放到支持 Skill 的环境中，然后显式调用：

```text
Use $scientific-coding 来完成这个编码任务。
```

也可以自然语言调用：

```text
请按科学 Coding 观处理这个任务：先读上下文，不编造 API，小步修改，并完成验证。
```

## 适用场景

- Bug 修复；
- 小功能开发；
- 代码重构计划；
- Code Review；
- 项目规范化协作；
- Agent 行为约束；
- 团队 AI 编程工作流统一。

## 最终原则

> AI 可以生成代码，但工程质量需要人和 AI 共同守护。
