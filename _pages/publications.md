---
layout: page
permalink: /publications/
title: publications
description: publications by categories in reversed chronological order. generated by jekyll-scholar.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->


<div style="counter-reset: paper-counter {% bibliography_count -f papers %}">
<div class="publications">

<h2>Conference & journal articles</h2>


{%- for y in page.years-paper %}
  <h2 class="year">{{y}}</h2>

  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
</div>


<div style="counter-reset: paper-counter {% bibliography_count -f preprints %}">
<div class="publications">

<h2>Preprints</h2>

<h2 class="year">&nbsp;</h2>
{% bibliography -f preprints %}
</div>
</div>
