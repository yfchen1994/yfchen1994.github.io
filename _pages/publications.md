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

{% assign current_year = 2100 %}
{% assign pub_year = 2100 %}
{% for post in site.publications reversed %}
  {% if post.collection == 'publications' %}
    {% assign pub_year = post.date | date: "%Y" | plus: 0 %}   
      {% if pub_year < current_year %}
        {% assign current_year = pub_year %}
        {% include display_year.html %}
      {% endif %}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}

