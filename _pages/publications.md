---
layout: page
permalink: /publications/
title: Publications
description: "*equal contributions"
years: [2023, 2021, 2020, 2019, 2018, 2014]
nav: true
nav_order: 1
---
Please refer to my [Google Scholar Profile](https://scholar.google.com/citations?user=8dxN6C8AAAAJ&hl=en&oi=ao) for the most up-to-date information.
<!-- _pages/publications.md -->
<div class="publications">
<!-- <p>* indicate equal contributions</p> -->


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
  console.log({% bibliography -f papers -q @*[year={{y}}]* %})
{% endfor %}

</div>
