---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

You can also find my articles on [my Google Scholar profile](https://scholar.google.com/citations?user=4gE_vYgAAAAJ).

<div class="pub-list">
  {% for p in site.data.all_publications %}
    {% include pub-item.html
      title=p.title
      authors=p.authors_html
      venue=p.venue
      badge=p.badge
      paper_url=p.paper_url
      code_url=p.code_url
      project_url=p.project_url
      dataset_url=p.dataset_url %}
  {% endfor %}
</div>
