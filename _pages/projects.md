---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

{% comment %}
{% for project in site.projects reversed %}
  <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
  <p>{{ project.excerpt }}</p>
{% endfor %}
{% endcomment %}


{% include base_path %}

{% for post in site.projects reversed %}
  {% include archive-single.html %}
{% endfor %}
