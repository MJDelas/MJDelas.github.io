---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022, 2020, 2019, 2017, 2015, 2013, 2009]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
