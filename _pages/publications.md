---
layout: page
permalink: /publications/
title: Publications
description: 
years: [2022, 2021, 2020, 2019, 2018, 2017, 2016]
nav: true
---

[[Preprint papers](#preprint-papers)] |  [[Conference papers](#conference-papers)] | [[Journal papers](#journal-papers)]

#### Preprint papers

<div class="publications">

{% for y in page.years %}
  {% bibliography -f preprint -q @*[year={{y}}]* %}
{% endfor %}

</div>

#### Conference papers

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f confs -q @*[year={{y}}]* %}
{% endfor %}

</div>

#### Journal papers

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journal -q @*[year={{y}}]* %}
{% endfor %}

</div>
