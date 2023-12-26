---
layout: page
title: "archive"
description: "文章"
header-img: "img/orange.jpg"
---


<ul class="listing">
{% for post in site.posts %}
  {% capture y %}{{post.date | date:"%Y"}}{% endcapture %}
  {% if year != y %}
    {% assign year = y %}
    <li class="listing-seperator">{{ y }}</li>
  {% endif %}
  <li class="listing-item">
    <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
    <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

阿壮:
那我也得了解一下吧

阿壮:
我老板做个网站花了二十几万

阿壮:
我靠我以后啥也不懂

阿壮:
一个网站也被人坑十几万

阿壮:
然后她一个朋友说，现在复制这个模板也就一万多块钱就能再做一个
