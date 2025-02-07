---
layout: default
title: "Blog"
permalink: /blog/
---

<!-- Blog Header Section -->
<div class="blog-header">
    <h1>My Blog</h1>
    <p>Welcome to my blog! Here, I share updates about my life, work, and projects.</p>
</div>

<!-- Blog Post List -->
<div class="blog-list">
    {% for post in site.posts %}
        <div class="blog-post">
            <span class="blog-date">{{ post.date | date: "%B %d, %Y" }}</span>
            <a href="{{ post.url }}" class="blog-title">{{ post.title }}</a>
        </div>
    {% endfor %}
</div>
