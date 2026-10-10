---
layout: default
title: "Writing"
permalink: /blog/
---

<section class="hero hero--sub">
  <p class="label">Notes &amp; updates</p>
  <h1 class="display display--md">Writing</h1>
</section>

<section class="section">
  {% if site.posts.size > 0 %}
  {% include post-list.html %}
  {% else %}
  <p class="muted">Nothing published yet.</p>
  {% endif %}
</section>
