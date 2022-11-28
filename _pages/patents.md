---
layout: page
permalink: /patents/
title: patents
description: patents in reverse chronological order.
years: [2022, 2023]
nav: false
nav_order: 2
---
<!-- _pages/patents.md -->
<div class="patents">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f patents -q @*[year={{y}}]* %}
{% endfor %}

</div>
