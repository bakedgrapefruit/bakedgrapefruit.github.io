---
layout: default
title: "Marketing"
description: 순간을 연결하여 함께 할 수 있는 가치를 찾아요.
main: true
project-header: true
header-img: img/about.jpg
---

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.marketing == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>
