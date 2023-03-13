---
layout: page
permalink: /publications/
title: publications
description: Here is a complete list of my publications. All of my publications can be found on my <a href='https://inspirehep.net/authors/1776885?ui-citation-summary=true'>InspireHEP profile</a> 
years: [2023,2022, 2017, 2016]
# years: [2022, 2017, 2016, 1967, 1956, 1950, 1935, 1905]
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
