---
layout: page
title: "Writing"
permalink: /writing/
nav: true
---

<style>
  .post-title {
    font-size: 0.75rem; /* Adjust this value as needed */
  }
</style>

{% for post in site.posts %}
<article>
  <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.excerpt }}</p>
</article>
{% endfor %}
