---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
redirect_from:
  - /publication/
  - /publication.html
---

You can also find my publications on [Google Scholar](https://scholar.google.com/citations?user=piVw5goAAAAJ&hl=en&oi=ao).

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

