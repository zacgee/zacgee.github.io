---
layout: default
title: "Index"
---

<section class="hero hero--portrait">
  <div class="hero__text">
    <p class="label">Programmer Analyst — First Citizens Bank</p>
    <h1 class="display">Zachary<br>Geelalsingh</h1>
  </div>
  <figure class="portrait">
    <img src="{{ "/assets/portrait.jpg" | relative_url }}" width="640" height="800" alt="Portrait of Zachary Geelalsingh">
    <figcaption class="label">Fig. 01</figcaption>
  </figure>
</section>

<section class="section">
  <h2 class="label"><span>01</span> About</h2>
  <div class="prose">
    <p>I'm a Programmer Analyst at First Citizens Bank in Trinidad and Tobago. Before that I studied Computer Science at Florida Institute of Technology. Outside of work I build web and mobile app. I enjoy figuring out the problem, shipping something, then making it simpler.</p>
    <p class="muted">Python · JavaScript · React · React Native · Node.js · SQL · Java · C++ · C</p>
  </div>
</section>

<section class="section">
  <h2 class="label"><span>02</span> Selected projects</h2>
  {% include project-list.html limit=4 %}
  {% if site.data.projects.size > 4 %}<p class="back"><a href="{{ "/projects/" | relative_url }}">All {{ site.data.projects.size }} projects →</a></p>{% endif %}
</section>

{% if site.posts.size > 0 %}
<section class="section">
  <h2 class="label"><span>03</span> Writing</h2>
  {% include post-list.html limit=3 %}
</section>
{% endif %}

<section class="section">
  <h2 class="label"><span>{% if site.posts.size > 0 %}04{% else %}03{% endif %}</span> Contact</h2>
  <ul class="links">
    <li><a href="mailto:{{ site.email }}">Email</a></li>
    <li><a href="https://github.com/{{ site.github }}">GitHub</a></li>
    <li><a href="https://www.linkedin.com/in/{{ site.linkedin }}">LinkedIn</a></li>
    <li><a href="{{ "/assets/Zachary_Resume.pdf" | relative_url }}">Résumé (PDF)</a></li>
  </ul>
</section>
