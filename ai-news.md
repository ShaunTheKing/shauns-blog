---
layout: default
title: Weekly AI News
permalink: /ai-news/
---
<header class="hero">
  <p class="eyebrow">Every week</p>
  <h1>Weekly AI News</h1>
  <p class="hero-sub">The biggest stories in AI, rounded up and explained in a few minutes.</p>
</header>

<section class="posts">
  {% assign issues = site.categories['ai-news'] %}
  {% if issues and issues.size > 0 %}
    {% for post in issues %}
    <a class="card" href="{{ post.url | relative_url }}">
      <time datetime="{{ post.date | date_to_xmlschema }}">Week of {{ post.date | date: "%B %-d, %Y" }}</time>
      <h2>{{ post.title }}</h2>
      <p>{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
      <span class="more">Read this week ›</span>
    </a>
    {% endfor %}
  {% else %}
    <div class="empty">
      <h2>First issue coming soon</h2>
      <p>Check back next week for the first roundup.</p>
    </div>
  {% endif %}
</section>
