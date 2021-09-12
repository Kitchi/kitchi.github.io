---
layout: page
permalink: /publications/
title: publications
description: a selection of papers toward which I have contributed
years: [2021, 2019, 2018]
nav: true
---

An up-to-date list can be found on [Google Scholar](https://scholar.google.com/citations?user=x7FWcr4AAAAJ)

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
