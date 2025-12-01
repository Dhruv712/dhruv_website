---
layout: page
title: "Travel"
permalink: /travel/
nav: true
---

<style>
  /* Match Writing page list styles */
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
    font-size: 1.3rem;
    font-family: 'Roboto', sans-serif;
  }
  .posts-list .post-title a {
    color: #000;
    text-decoration: none;
  }
  .posts-list .post-date {
    font-size: 0.9rem;
    color: #666;
    font-family: 'Roboto', sans-serif;
  }
</style>

<div class="posts-list">
    {% assign sorted_travel = site.travel | sort: 'date' | reverse %}
    {% for trip in sorted_travel %}
    <article class="post">
      <div class="post-header">
        <h2 class="post-title"><a href="{{ trip.url }}">{{ trip.title }}</a></h2>
        <span class="post-date">{{ trip.date | date: "%B %Y" }}</span>
      </div>
    </article>
    {% endfor %}
  </div>
