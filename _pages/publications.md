---
layout: page
permalink: /publications/
title: Publications
# description: Publications by categories in reversed chronological order.
years-paper: [2022, 2021, 2020, 2019]
# years-preprint: [2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<h2>Conference & journal articles</h2>

{%- for y in page.years-paper %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<div class="publications">

<h2>Preprints</h2>

{% bibliography -f preprints %}

</div>
