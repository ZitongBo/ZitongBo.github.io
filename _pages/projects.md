---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

{% include lang-style.html %}

<div class="lang-block-en" markdown="1">

## Embodied AI Projects

My recent work at Xiaomi Robotics Lab focuses on data, models, agents, and real-robot systems for embodied intelligence.

### Embodied Self-Evolution System

I am exploring a closed loop between agents, real robots, and human collaboration. The system turns high-level goals into executable robot policies, evaluates what happens in the physical world, and uses both successful and failed attempts to inform the next iteration.

The work covers system design, task adaptation, safety boundaries, data return, and real-robot validation. It combines Code-as-Policy with robot APIs and VLA capabilities, with agents responsible for analyzing failures, revising plans, and retrying tasks.

### Ego-UMI Data Pipeline and Mask-Aware VLA Policies

I led the end-to-end workflow for egocentric human manipulation data: collection, automatic annotation, quality control, and policy training. The pipeline processes task videos, extracts keyframes, corrects fisheye imagery, and uses vision-language grounding and segmentation models to annotate objects and task-relevant regions.

By masking hands and arms in human demonstrations, the work reduces the visual gap between egocentric demonstrations and robot deployment. The resulting data supports mask-aware robot policies and has been used in Xiaomi-Robotics-1.

### Embodied VLM Pretraining and Post-training

I helped build an embodied VLM workflow from pretraining and post-training through evaluation and real-robot use. It combines general vision-language learning with robot-task supervision and reasoning-oriented post-training to improve spatial understanding, planning, progress monitoring, failure detection, and tool use.

This work also supported MiMo-Embodied with the Xiaomi EV team, including applications in reward evaluation, grasp-and-place localization, and agent task decomposition.

### Embodied Agent System

As the system algorithm lead, I designed an Agent-and-Tool execution architecture that connects models, tools, and real robots through clear interfaces and acceptance criteria. The agent handles instruction understanding, task decomposition, and memory, while the tool layer exposes capabilities such as grounding, navigation, perception, and robot control.

The system integrates VLN and VLA policies on fixed-arm and mobile dual-arm platforms, supporting real-world tasks that combine navigation, manipulation, and multi-step execution.

</div>

<div class="lang-block-zh" markdown="1">

## 具身智能项目

我在小米机器人实验室的工作，主要围绕具身智能的数据、模型、Agent 与真机系统展开。

### 具身自进化系统

我在探索 Agent、真机与人协同构成的闭环系统：Agent 将高层任务目标转化为可执行的机器人策略，系统根据真实环境中的执行结果进行评估，并将成功与失败的经验用于下一轮迭代。

相关工作涵盖总体架构、任务适配、安全边界、数据回流和真机验证。系统结合 Code-as-Policy、机器人 API 与 VLA 能力，由 Agent 负责分析失败原因、调整方案并重新尝试。

### Ego-UMI 数据构建与带 Mask VLA 策略训练

我负责 ego 视角人类操作数据的完整流程，包括数据采集、自动标注、质量验收和策略训练。数据流程涵盖任务视频处理、关键帧抽取、鱼眼图像校正，以及利用视觉语言定位与分割模型标注物体和任务相关区域。

通过对人手和手臂进行 mask，这项工作尝试缩小人类演示与机器人部署之间的视觉差距。产出的数据可用于训练带 Mask 的机器人策略，并已被 Xiaomi-Robotics-1 使用。

### 具身 VLM 预训练与后训练

我参与搭建从预训练、后训练、评测到真机应用的具身 VLM 流程。该流程将通用视觉语言能力、机器人任务监督和面向推理的后训练结合起来，提升模型在空间理解、任务规划、进度监控、失败检测和工具调用上的能力。

相关工作也支撑了与 Xiaomi EV 团队合作的 MiMo-Embodied，并应用于奖励评估、抓放区域定位和 Agent 任务拆解等方向。

### 具身 Agent 系统

作为系统算法负责人，我设计了连接模型、工具和真机的 Agent-Tool 执行架构，并明确各模块之间的接口和验收标准。Agent 负责理解指令、拆解任务与维护记忆；工具层则提供目标定位、导航、感知和机器人控制等能力。

该系统将 VLN 和 VLA 策略接入固定臂与轮式双臂平台，支持导航、操作和多步骤任务的协同执行。

</div>
