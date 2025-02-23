---
layout: page
title: "Writing"
permalink: /writing/
nav: true
---

<style>
  .posts-list h2 {
    font-size: 1.5rem; /* Adjust the size for post titles only */
  }
</style>

<div class="posts-list">
  {% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
  </article>
  {% endfor %}
</div>
