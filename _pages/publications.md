---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order. Also see this <a href="https://scholar.google.com/citations?user=ncBRYIUAAAAJ&hl=en">Google Scholar</a> page.
years_pre: [2021]
years_pub: [2021,2020]
nav: true
---

<br />







### Preprints



<div class="publications">

{% for y in page.years_pre %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}},abbr=ArXiv] %}
{% endfor %}

</div>




*******
<br />





### Conference Papers



<div class="publications">

{% for y in page.years_pub %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}},abbr!=ArXiv] %}
{% endfor %}

</div>

