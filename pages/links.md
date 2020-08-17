---
layout: page
title: Links
description: 没有链接的博客是孤独的
keywords: 友情链接
comments: true
menu: 链接
permalink: /links/
---

<script src="https://cdn.jsdelivr.net/npm/jquery/dist/jquery.min.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/font-awesome/css/font-awesome.min.css"/>
<script src="https://cdn.jsdelivr.net/gh/stevenjoezhang/live2d-widget/autoload.js"></script>

> 建议收藏的好东西

<ul>
{% for link in site.data.links %}
  {% if link.src == 'life' %}
  <li><a href="{{ link.url }}" target="_blank">{{ link.name}}</a></li>
  {% endif %}
{% endfor %}
</ul>

> 友情链接

<ul>
{% for link in site.data.links %}
  {% if link.src == 'www' %}
  <li><a href="{{ link.url }}" target="_blank">{{ link.name}}</a></li>
  {% endif %}
{% endfor %}
</ul>
