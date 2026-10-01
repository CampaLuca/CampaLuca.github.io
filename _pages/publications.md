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

<br>
<h2 class="bibliography" style="color: var(--global-text-color); border-bottom: 1px solid var(--global-divider-color);
  padding-top: 1rem;
  margin-top: 2rem;
  text-align: left;">Peer Reviewed</h2>
<div class="publications">

{% bibliography --query @*[preprint=no]* %}

</div>
<br>

<h2 class="bibliography" style="color: var(--global-text-color); border-bottom: 1px solid var(--global-divider-color);
  padding-top: 1rem;
  margin-top: 2rem;
  text-align: left;">Preprints</h2>

<div class="publications">
  {% bibliography --query @*[preprint=yes]* %}
</div>
