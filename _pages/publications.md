---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order. Full list can be found at <b><a href='https://scholar.google.com.hk/citations?user=8Of_NYQAAAAJ&hl=en'>Google Scholar</a></b></br />. <b>* indicates equal contribution, ** indicates corresponding author.</b><br />
years: [2023, 2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
