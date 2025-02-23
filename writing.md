---
layout: page
title: "Writing"
permalink: /writing/
nav: true
---

<style>
  .posts-list .post-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding: 0.5rem 0;
    border-bottom: 1px solid #ddd;
    margin-bottom: 1rem;
  }
  .posts-list .post-title {
    margin: 0;
    font-size: 1.5rem;
    font-family: Arial, sans-serif;
  }
  .posts-list .post-title a {
    color: #000; /* black text */
    text-decoration: none;
  }
  .posts-list .post-date {
    font-size: 0.9rem;
    color: #666;
    font-family: Arial, sans-serif;
  }
</style>

<div class="posts-list">
  {% for post in site.posts %}
  <article class="post">
    <div class="post-header">
      <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <span class="post-date">{{ post.date | date: "%B %d, %Y" }}</span>
    </div>
  </article>
  {% endfor %}
</div>
