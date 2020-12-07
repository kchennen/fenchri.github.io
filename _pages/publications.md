---
layout: page
permalink: /publications/
title: publications
index: 2
sections: [Conference Papers, Journals, Workshop Papers, Theses]
nav: true
---

You can also check my [Google Scholar](https://scholar.google.co.uk/citations?user=nVKZdJkAAAAJ&hl=en&authuser=1) page.

<div class="publications">

{% for y in page.sections %}
  <h2 class="section">{{y}}</h2>
  {% bibliography -f papers -q @*[section={{y}}]* %}
{% endfor %}

</div>


