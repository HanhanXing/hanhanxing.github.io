---
#layout: page #minima主题时期的
layout: categories # 换成Jeffrey的主题也许要改动的，update in 24-11-20
title: 🛒 分类
permalink: /categories/
---
<style>
.post-title {display: none;}
</style>
<div style="margin-top: 100px;"></div>

## **🛒 文章分类**
<div style="margin-top: 100px;"></div>
<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <div id="#{{ category_name | slugize }}"></div>
    <p></p>

    <h3 class="category-head">{{ category_name }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories[category_name] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>


---

### 本站标签一览表（Tags / Categories）  
更新时间：2024-11-03  

| All Tags    | Categories（分类）  |
|---------|-----------------------|
| Tech    | Technology（科技）        |
| SocSci  | Social Sciences（社会科学）|
| Fin     | Finance（金融）           |
| Phil    | Philosophy（哲学）        |
| Biz     | Business（商业）          |
| Prog    | Programming（编程）       |
| Math    | Mathematics（数学）       |
| Gaming  | Gaming（游戏）            |
| Health  | Health（健康）            |
| Poli    | Politics（政治）          |
| Arts    | Arts（艺术）              |
| Hist    | History（历史）           |
| Lit     | Literature（文学）        |
| Edu     | Education（教育）         |
| LifeStyle | Lifestyle（生活方式） |
| Sci     | Science（科学）        |
| Law       | Law（法律）          |
| Psych     | Psychology（心理学）  X|
| Econ      | Economics（经济学）  X |
| Sports  | Sports（体育）        X    |
| Env     | Environment（环境）   X    |
| Culture | Culture（文化）       X    |
| Eng     | Engineering（工程）   X    |
| Trav      | Travel（旅行）  X    |
| FinTech | Fin-Tech（金融科技）    X   |