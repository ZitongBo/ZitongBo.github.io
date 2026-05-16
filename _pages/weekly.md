---
layout: archive
title: "Weekly"
permalink: /weekly/
author_profile: true
---

{% include lang-style.html %}

<div class="lang-block-en">
<p>Weekly digest focused on embodied intelligence, robot manipulation, and multimodal large models.</p>
</div>
<div class="lang-block-zh">
<p>聚焦具身智能、机器人操作与多模态大模型，每周整理值得关注的论文、进展和思考。</p>
</div>

<ul>
{% assign weekly_posts = site.posts | where_exp: "post", "post.categories contains 'weekly'" %}
{% for post in weekly_posts %}
  <li>
    <a href="{{ post.url }}"><strong>{{ post.title }}</strong></a>
    <span style="color: #7a8288; font-size: 0.85em; margin-left: 8px;">{{ post.date | date: "%Y-%m-%d" }}</span>
    {% if post.excerpt %}
      <p style="margin: 4px 0 12px; color: #555;">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    {% endif %}
  </li>
{% endfor %}
{% if weekly_posts.size == 0 %}
  <li style="color: #7a8288;">
    <span class="lang-block-en">First issue coming soon.</span>
    <span class="lang-block-zh">第一期即将发布，敬请期待。</span>
  </li>
{% endif %}
</ul>
