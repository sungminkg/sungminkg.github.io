---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

<!-- {% include youtube.html id="dnfslIC5CPg" %} -->
{% for project in site.projects %}
  <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
  <p>{{ project.excerpt }}</p>
{% endfor %}

{% include youtube.html id="dnfslIC5CPg" %}
