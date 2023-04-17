---
layout: page
permalink: /publications/
title: Research
description: 
years: [1967, 1956, 1950, 1935, 1905]
categories: ['Working Papers', 'Work in Progress', 'Publications', 'Other']
catprint: ['','Working Papers', 'Work in Progress', 'Publications', 'Other']
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
