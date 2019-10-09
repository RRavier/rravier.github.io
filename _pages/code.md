---
layout: archive
title: "Software I've Written"
permalink: /code/
author_profile: true
---

On this page, I will give links to the publically released packages I offer and maintain. Open source, reproducible science is important to me, and I try to spend a lot of time making everything I release something that I can be proud of releasing and that anyone using my packages can be proud of doing so.

Some of these are major, some of these are not. I stand by all of it, whatever the size, whatever the scope.

{% include base_path %}

{% for post in site.code reversed %}
  {% include archive-single.html %}
{% endfor %}
