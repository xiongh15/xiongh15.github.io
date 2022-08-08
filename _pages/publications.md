---
layout: page
permalink: /publications/
title: Publications
description: <b>*</b> indicates equal contribution.
years: [2022, 2021, 2020, 2019]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<script async src="https://badge.dimensions.ai/badge.js" charset="utf-8"></script>
<script type='text/javascript' src='https://d1bxh8uas1mnw7.cloudfront.net/assets/embed.js'></script>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
 {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
