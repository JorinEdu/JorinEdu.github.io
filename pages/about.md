---
layout: page
title: About
description: 始终如一
keywords: Jhon Woo
comments: true
menu: 关于
permalink: /about/
---

乔琳教育，是始终如一的学生英语教育品牌，致力于为中国的学生提供优质的个性化英语教学服务。

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
