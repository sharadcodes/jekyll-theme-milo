---
layout: default
permalink: /categories/
title: Categories
---

<div id="archives">
{% for category in site.categories %}
  <div class="archive-group">
    {% capture category_name %}{{ category | first }}{% endcapture %}
    <h4 class="category-head" id="{{ category_name | slugize }}">{{ category_name }}</h4>
     {% for post in site.categories[category_name] %}
       <article class="archive-item">
      <h6> :black_small_square:<a style="background-color:#F0F0F0; margin-bottom:2px;" href="{{site.baseurl}}{{ post.url }}">{{post.title}}</a></h6>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>
