---
layout: page
permalink: /publications/
title: Publications
description: 
nav: true # comment in case you don't want this page
nav_order: 2 # comment in case you don't want this page
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include publications/bib_search.liquid %}


## Peer Reviewed
<div class="publications">

{% bibliography --query @*[preprint=no]* %}

</div>



## PrePrint

<div class="publications">
  {% bibliography --query @*[preprint=yes]* %}
</div>
