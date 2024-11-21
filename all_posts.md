---
# layout: page （minima主题时期的，all_posts用的是minima里专门的一个‘page’布局，jeffery的主题中，类似all_posts的就直接挪用archives吧。
layout: articles # 换成Jeffrey的主题也许要改动的，update in 24-11-20
title: 📝 全部笔记
permalink: /all_posts/
# show_excerpts: true
---
<style>
.post-title {display: none;}
</style>
<div style="margin-top: 10px;"></div>

## **📝 全部笔记**
<div style="margin-top: 50px;"></div>
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

<div style="margin-top: 100px;"></div>
  
