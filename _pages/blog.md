---
permalink: /blog/
title: "Blog"
layout: single
author_profile: true
---

{% include lang-style.html %}

<div class="lang-block-en" markdown="1">

Technical articles on embodied intelligence, robotics, VLA, and AI industry trends.

## Zhihu Articles

- **[Reinforced Embodied Planning with Verifiable Reward for Real-World Robotic Manipulation](https://zhuanlan.zhihu.com/p/1966932514057724104)**
  How the REVER framework fine-tunes VLM planners with verifiable rewards to keep long-horizon manipulation reliable in the real world.

- **[Embodied Foundation Model](https://zhuanlan.zhihu.com/p/1969874282386560574)**
  A 2025 snapshot of representative embodied foundation models — Cosmos-Reason1, Magma, VeBrain, RoboBrain, Embodied-R1.

- **[AgiBot GO-1: The Evolution of Generalist Embodied Foundation Model from VLA to ViLLA](https://zhuanlan.zhihu.com/p/1920515230280189587)**
  How AgiBot GO-1 upgrades from VLA to ViLLA: capability transfer, hardware-software co-design.

- **[DeepSeek-V3: The Strongest Open-Source Foundation Model](https://zhuanlan.zhihu.com/p/21725843952)**
  Architecture, training stack, and benchmark wins.

- **[Real-Time Intelligent Systems](https://zhuanlan.zhihu.com/p/717190037)**
  How real-time constraints intersect with AI pipelines for safety-critical robots.

## Blog Posts

</div>

<div class="lang-block-zh" markdown="1">

聚焦具身智能、机器人、VLA 与 AI 行业趋势的技术文章。

## 知乎文章

- **[Reinforced Embodied Planning with Verifiable Reward for Real-World Robotic Manipulation](https://zhuanlan.zhihu.com/p/1966932514057724104)** / 《具身规划》
  介绍 REVER 框架，如何让 VLM 从"看得懂"走向"做得对"。

- **[Embodied Foundation Model](https://zhuanlan.zhihu.com/p/1969874282386560574)** / 《具身基座模型》
  概览 2025 年代表性具身基座模型。

- **[AgiBot GO-1](https://zhuanlan.zhihu.com/p/1920515230280189587)** / 《智元机器人 AgiBot GO-1》
  分析 AgiBot GO-1 如何从 VLA 升级到 ViLLA。

- **[DeepSeek-V3](https://zhuanlan.zhihu.com/p/21725843952)** / 《最强开源大模型 DeepSeek-V3》
  体系结构、训练栈与基准成绩。

- **[Real-Time Intelligent Systems](https://zhuanlan.zhihu.com/p/717190037)** / 《实时智能系统》
  实时约束与智能系统流程的耦合。

## 博客文章

</div>

<ul>
{% assign blog_posts = site.posts | where_exp: "post", "post.categories contains 'blog'" %}
{% for post in blog_posts %}
  <li>
    <a href="{{ post.url }}"><strong>{{ post.title }}</strong></a>
    <span style="color: #7a8288; font-size: 0.85em; margin-left: 8px;">{{ post.date | date: "%Y-%m-%d" }}</span>
    {% if post.excerpt %}
      <p style="margin: 4px 0 12px; color: #555;">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>
