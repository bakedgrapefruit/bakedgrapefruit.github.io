---
layout: default
title: "Experience"
description: 갖가지 경험들
main: true
project-header: true
header-img: img/about.jpg
---

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.experience == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>
