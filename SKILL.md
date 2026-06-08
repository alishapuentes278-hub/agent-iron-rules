---
name: agent-iron-rules
description: 【强制预加载】Agent 操作铁律 — 在任何毕业设计相关任务启动时必须与 grad-design-squad 同时加载。六大节覆盖所有工作流：范围控制、危险操作确认、沟通规则、记忆与背景、Karpathy 四原则、与 Agent Team 架构的集成约束。这不是参考建议，是硬约束——不加载=无规则裸跑。与 grad-design-squad 是并列的操作系统层 skill。
---

# Agent 操作铁律

> ⚠️ **本 skill 是硬约束，不是参考建议。** 启动任何毕业设计任务时，必须与 `grad-design-squad` 同时加载。铁律覆盖所有 Squad、所有任务、所有工作流，不加载意味着 Agent 不知道操作边界。
>
> 本 skill 与 `grad-design-squad` 的关系: grad-design-squad 定义"谁做什么、怎么协调"，agent-iron-rules 定义"怎么做才是对的"。

## 强制预加载规则

**每次启动毕业设计任务时，必须同时加载本 skill 和 grad-design-squad:**

```
用户触发 → 加载 grad-design-squad（建立 Squad 架构）
         → 加载 agent-iron-rules（建立操作边界）
         → 两者就绪后才开始执行
```

六节铁律概览:

| 节 | 核心原则 |
|----|---------|
| 一、范围控制 | 只改该改的 / 大改前确认 / 改完列清单 |
| 二、危险操作确认 | 破坏性操作先停 / 高危操作立墙 / 替我操作先问 |
| 三、沟通规则 | 拒绝废话 / 先给选项 / 不确定直说 / 篇幅看需求 |
| 四、记忆与背景 | 建立 MEMORY.md + ERRORS.md + 永久铁律 |
| 五、核心原则 | Karpathy 四原则：要问别假设 / 先最简单 / 别碰无关 / 标注不确定 |
| 六、集成约束 | 用户决策检查点 / 危险操作门禁 / 改动清单协议 / ERRORS.md / 全域只改该改的 |

## 参考文件导航

| 文件 | 内容 | 何时加载 |
|------|------|---------|
| [rules.md](references/rules.md) | 完整六大节铁律 + 集成约束 + 改动清单协议 + ERRORS.md 格式 | 随 skill 加载时读取（强制）|
| [reporting-protocol.md](references/reporting-protocol.md) | 工作流运行报告协议 + 进度播报铁律 | 随 skill 加载时读取 |
