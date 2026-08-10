---
layout: single
title: "AI Coding"
permalink: /ai-coding/
author_profile: true
---

{% include lang-style.html %}

<div class="lang-block-en" markdown="1">

I rely heavily on AI coding tools (Claude Code, Cursor, etc.) in my daily work and research. Here I document real-world cases and reflections.

## Tools

- **Claude Code** — Primary tool for code generation, refactoring, debugging, and documentation
- **Cursor** — Codebase-aware editor, ideal for large projects
- **GitHub Copilot** — Lightweight everyday completion

---

## Case Studies

### Building This Site with Claude Code
**Tool:** Claude Code
**Context:** Building this Jekyll academic site from scratch — adding pages, tweaking styles, fixing config errors
**Takeaway:** AI grasps Jekyll template structure quickly, cutting down time spent reading docs. Especially effective for niche syntax like Liquid templates.

---

### Debugging Robot Simulation Environments
**Tool:** Claude Code + Cursor
**Context:** Debugging VLA policies in IsaacSim / MuJoCo, pinpointing sensor data alignment issues
**Takeaway:** Feeding error messages and env configs together to the AI locates issues in minutes that would otherwise take hours.

---

### Paper Writing Assistance
**Tool:** Claude
**Context:** Polishing Abstract and Related Work sections for the REVER paper
**Takeaway:** AI cannot replace thinking, but it significantly improves language quality. Asking AI to critique first, then revise, works better than asking it to rewrite directly.

---

### Codex + GPT5.5 Goal-Driven Agent 实验
**工具：** Codex CLI + GPT5.5 Goal 模式
**场景：** 让 AI agent 自主执行具身智能研究的完整流程——搭建环境、跑基线、读日志、归因失败、生成数据、训练模型、提交评测、汇总结果并持续迭代（跑了 15 天）
**核心思路：** 将 Codex 反复调用的能力封装为可复用的 skill（镜像管理、数据平台、模型训练、评测、论文检索、知识库检索），使其能围绕同一研究目标持续执行
**关键成果：**
- 自动跑通 4 个 benchmark（ALFWorld、EB-ALFRED、EB-Habitat、LoTa-WAH）
- 复现 RoboAgent-style pipeline，建立可比较的 baseline
- 从 rollout 和日志中自动归因失败（重复搜索、阶段混乱、记忆未利用、工具格式错误等）
- 通过 SFT/DPO 将失败轨迹转化为训练信号
- 设计 Public-Sitter Memory 机制，只记录公开交互历史，可审计
**收获：** Prompt 是接口约束，不是具身大脑能力本身；真正的长程状态保持、多目标 bookkeeping、复杂工具链切换，需要结合训练来解决

---

## Reflections

> AI Coding is not about writing less code — it's about spending your time on decisions that actually matter.

The core skill for engineers using AI tools has shifted to: **clearly describing the problem**, **judging output quality**, and **keeping the big picture in mind**. This maps closely to what robotics research demands — you need to know what the robot should do before you can verify whether it did it right.

---

*Continuously updated. Feel free to reach out by email if a specific use case interests you.*

</div>

<div class="lang-block-zh" markdown="1">

我在日常工作和研究中大量使用 AI Coding 工具（Claude Code、Cursor 等），这里记录一些真实的实践案例和使用心得。

## 工具

- **Claude Code** — 主力工具，用于代码生成、重构、调试和文档撰写
- **Cursor** — 结合 codebase 上下文的编辑器，适合大型项目
- **GitHub Copilot** — 日常轻量补全

---

## 实践案例

### 用 Claude Code 搭建个人主页
**工具：** Claude Code
**场景：** 从零开始搭建这个 Jekyll 学术主页，包括新增页面、调整样式、修复配置错误
**收获：** AI 能快速理解 Jekyll 模板结构，大幅减少查文档的时间；对于 Liquid 模板语法这类"冷门"知识，效果尤其好

---

### 机器人仿真环境调试
**工具：** Claude Code + Cursor
**场景：** 在 IsaacSim / MuJoCo 环境中调试 VLA 策略，快速定位传感器数据对齐问题
**收获：** 将报错信息和环境配置一起喂给 AI，能在几分钟内定位原本需要一两小时排查的问题

---

### 论文写作辅助
**工具：** Claude
**场景：** REVER 论文的 Abstract、Related Work 润色与逻辑梳理
**收获：** AI 不能替代思考，但能显著提升语言质量；让 AI 先给出批评意见再修改，比直接让它重写效果更好

---

### Codex + GPT5.5 Goal-Driven Agent 实验
**工具：** Codex CLI + GPT5.5 Goal 模式
**场景：** 让 AI agent 自主执行具身智能研究的完整流程——搭建环境、跑基线、读日志、归因失败、生成数据、训练模型、提交评测、汇总结果并持续迭代（跑了 15 天）
**核心思路：** 将 Codex 反复调用的能力封装为可复用的 skill（镜像管理、数据平台、模型训练、评测、论文检索、知识库检索），使其能围绕同一研究目标持续执行
**关键成果：**
- 自动跑通 4 个 benchmark（ALFWorld、EB-ALFRED、EB-Habitat、LoTa-WAH）
- 复现 RoboAgent-style pipeline，建立可比较的 baseline
- 从 rollout 和日志中自动归因失败（重复搜索、阶段混乱、记忆未利用、工具格式错误等）
- 通过 SFT/DPO 将失败轨迹转化为训练信号
- 设计 Public-Signal Memory 机制，只记录公开交互历史，可审计
**收获：** Prompt 是接口约束，不是具身大脑能力本身；真正的长程状态保持、多目标 bookkeeping、复杂工具链切换，需要结合训练来解决

---

## 一些感受

> AI Coding 不是让你少写代码，而是让你把时间花在真正重要的决策上。

工程师用 AI 工具的核心能力，变成了：**清晰描述问题**、**判断输出质量**、**把握整体方向**。这和做机器人研究需要的能力高度重合——你得知道机器人应该做什么，才能验证它做对了没有。

---

*持续更新中。如果你对某个具体场景感兴趣，欢迎通过邮件交流。*

</div>
