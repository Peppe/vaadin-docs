---
layout: page
title: Instructions
---
<h2>normal content</h2>
{% for post in site.posts %}
<div class="post">
<h1 class="post-title">
  <a href="{{ post.url }}">
    {{ post.title }}
  </a>
</h1>

<span class="post-date">{{ post.date | date_to_string }}</span>

{{ post.content }}
</div>
{% endfor %}