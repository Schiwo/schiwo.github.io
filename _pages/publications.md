---
layout: page
permalink: /publications/
title: publications
description: publications in reversed chronological order.
nav: true
nav_order: 2
years: ["preprint", 2026, 2024, 2023, 2022, 2021]
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{ y }}</h2>
  {% bibliography -q @*[year={{y}}]* %}
{%- endfor %}

</div>