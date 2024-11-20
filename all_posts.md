---
# layout: page （minima主题时期的，疑似all_posts是minima专门的一个布局，jeffery的主题不需要这个文档。在gigignore和_config.yml里把它去掉先吧。。。
layout: all_posts # 换成Jeffrey的主题也许要改动的，update in 24-11-20
title: 📝 全部笔记
permalink: /all_posts/
# show_excerpts: true
---
<style>
.post-title {display: none;}
</style>
<div style="margin-top: 100px;"></div>

## **📝 全部笔记**
<div style="margin-top: 100px;"></div>
<!-- All Posts Section -->
<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      <h3>
        <a class="post-link" href="{{ post.url }}">{{ post.title | escape }}</a>
      </h3>
    </li>
  {% endfor %}
</ul>
  
