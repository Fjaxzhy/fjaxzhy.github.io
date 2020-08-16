---
layout: page
title: About
description: 愿我们能在更开放的平行世界相遇
keywords: 神楽弥生, KaguraYayoi, kagurayayoi, 神乐弥生
comments: true
menu: 关于
permalink: /about/
---
一个专业是物联网的喜欢写程序的肥宅

主要使用C# Java和C++也稍微会些

最近在搞Bot和学习Python

目前方向是Telegram.Bot和Mirai.Bot

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}


{% if site.url contains 'mazhuang.org' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ assets_base_url }}/assets/images/qrcode.jpg" alt="闷骚的程序员" />
</li>
{% endif %}
</ul>


## Skill 

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
