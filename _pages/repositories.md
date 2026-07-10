---
layout: page
permalink: /repositories/
title: Repositories
description: Selected open-source repositories from my research.
nav: true
nav_order: 4
---

{% if site.data.repositories.repos %}
<div class="repo-grid">
  {% for repo in site.data.repositories.repos %}
  <a class="repo-card" href="{{ repo.url }}" target="_blank" rel="external nofollow noopener">
    <span class="repo-card-head"><span class="repo-owner">jae-hlee /</span> <span class="repo-name">{{ repo.name }}</span></span>
    <span class="repo-card-desc">{{ repo.description }}</span>
  </a>
  {% endfor %}
</div>
{% endif %}
