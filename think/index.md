---
layout: default
title: "단상"
description: 생각나는 대로의 단편적인 생각
main: true
project-header: true
header-img: img/about.jpg
---

<ul class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.think == true %}
{% include post-list.html %}
{% endif %}
{% endfor %}
</ul>
