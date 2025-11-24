---
title: "Reinforced Embodied Planning with Verifiable Reward for Real-World Robotic Manipulation"
collection: publications
category: manuscripts
permalink: /publication/REVER
excerpt: 'Authors: **Zitong Bo**, Yue Hu, Jinming Ma, Mingliang Zhou, Junhui Yin, Yachen Kang, Yuqi Liu, Tong Wu, Diyun Xiang, Hao Chen'
date: 2025-09-25
venue: 'arXiv preprint'
paperurl: 'https://arxiv.org/abs/2509.25852'
citation: 'Bo, Z., Hu, Y., Ma, J., Zhou, M., Yin, J., Kang, Y., Liu, Y., Wu, T., Xiang, D., & Chen, H. (2025). Reinforced Embodied Planning with Verifiable Reward for Real-World Robotic Manipulation. arXiv preprint arXiv:2509.25852.'
---

Enabling robots to execute long-horizon manipulation tasks from free-form language instructions remains a fundamental challenge in embodied AI. While vision-language models (VLMs) have shown promise as high-level planners, their deployment in the real world is hindered by two gaps: (i) the scarcity of large-scale, sequential manipulation data that couples natural language with multi-step action plans, and (ii) the absence of dense, interpretable rewards for fine-tuning VLMs on planning objectives. To address these issues, we propose REVER, a framework that empowers VLMs to generate and validate long-horizon manipulation plans from natural language instructions in real-world scenarios. Under REVER we train and release RoboFarseer, a VLM incentivized to emit chain-of-thought that perform temporal and spatial reasoning, ensuring physically plausible and logically coherent plans. To obtain training data, we leverage the Universal Manipulation Interface framework to capture hardware-agnostic demonstrations of atomic skills. An automated annotation engine converts each demonstration into vision-instruction-plan triplet. We introduce a verifiable reward that scores the generated plan by its ordered bipartite matching overlap with the ground-truth skill sequence. At run time, the fine-tuned VLM functions both as a planner and as a monitor, verifying step-wise completion. RoboFarseer matches or exceeds the performance of proprietary models that are orders of magnitude larger, while on open-ended planning it surpasses the best baseline by more than 40%. In real-world, long-horizon tasks, the complete system boosts overall success by roughly 60% compared with the same low-level controller without the planner. We will open-source both the dataset and the trained model upon publication.

