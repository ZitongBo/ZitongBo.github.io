---
layout: archive
title: "Experience"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include lang-style.html %}
{% include base_path %}

<div class="lang-block-en" markdown="1">

## Education

* Ph.D, Institute of Software, Chinese Academy of Sciences, 2018–2024
  * Real-time Systems, Embedded AI
  * Advisor: Prof. [Ying Qiao](https://people.ucas.ac.cn/~yqiao)
* B.S., School of Computer & Communication Engineering, University of Science & Technology Beijing, 2014–2018

## Work Experience

* 2024–present: Xiaomi Robotics Lab
  * Senior Algorithm Engineer
  * Vision-Language-Action Models (VLA), Agentic AI, Chain-of-Thought, Reinforcement Learning
* 2017–2018: Institute of Automation, Chinese Academy of Sciences
  * Research Intern
  * Reinforcement Learning, Game Theory
  * Advisor: Prof. [Junliang Xing](https://pi.cs.tsinghua.edu.cn/lab/people/jlxing/en/)

## Publications

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

</div>

<div class="lang-block-zh" markdown="1">

## 教育经历

* 博士，中国科学院软件研究所，2018–2024
  * 研究方向：实时系统、嵌入式 AI
  * 导师：[乔颖](https://people.ucas.ac.cn/~yqiao) 研究员
* 学士，北京科技大学计算机与通信工程学院，2014–2018

## 工作经历

* 2024–至今：小米机器人实验室
  * 高级算法工程师
  * 研究方向：视觉-语言-动作模型（VLA）、具身智能体、思维链、强化学习
* 2017–2018：中国科学院自动化研究所
  * 科研实习生
  * 研究方向：强化学习、博弈论
  * 合作导师：[邢军亮](https://pi.cs.tsinghua.edu.cn/lab/people/jlxing/en/) 研究员

## 论文发表

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

</div>
