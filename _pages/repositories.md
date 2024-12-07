---
layout: page
permalink: /repositories/
title: Repositories
description: 
nav: true # comment in case you don't want this page
nav_order: 4 # comment in case you don't want this page
---

{% if site.github_username %}


<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% include repository/repo_user.liquid username=site.github_username %}
</div>
{% endif %}

---

{% if site.github_repos %}

## Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
