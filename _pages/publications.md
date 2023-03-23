---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order. Included all the Books, Papers, Articles and chapters in book.
years: [1998,1999,2000,2003,2008,2009,2010,2011,2012,2013,2014,2015,2016,2017,2018,2020,2021,2023]
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
