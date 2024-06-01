---
layout: base
title: 📝 全部笔记
permalink: /all_posts/
# show_excerpts: true
---
<div style="margin-top: 50px;"></div>
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
  
