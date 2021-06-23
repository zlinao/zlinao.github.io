---
layout: page
permalink: /publications/
title: Publications
description: Check the full publications <a href="https://scholar.google.co.uk/citations?user=cPtgl3wAAAAJ&hl=en"><b>here</b></a>
years: [2021,2020,2019]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
