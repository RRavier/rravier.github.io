---
layout: archive
permalink: /projects/
author_profile: true
---

{% if author.googlescholar %}
  My <u><a href="{{author.googlescholar}}">Google Scholar profile</a></u> contains links to most (but not all) of my papers, though there are some things missing from there. You can find synopses of my work in this section.
{% endif %}

{% include base_path %}

{% for post in site.projects reversed %}
  {% include archive-single.html %}
{% endfor %}
