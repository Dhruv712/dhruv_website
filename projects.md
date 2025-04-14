---
layout: page
title: "Writing"
permalink: /writing/
nav: true
---

<style>
  .projects-list .project-header {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding: 0.5rem 0;
    border-bottom: 1px solid #ddd;
    margin-bottom: 1rem;
  }
  .projects-list .project-title {
    margin: 0;
    font-size: 1.3rem;
    font-family: 'Roboto', sans-serif;
  }
  .projects-list .project-title a {
    color: #000; /* black text */
    text-decoration: none;
  }
  .projects-list .project-date {
    font-size: 0.9rem;
    color: #666;
    font-family: 'Roboto', sans-serif;
  }
</style>

<div class="projects-list">
  {% for project in site.projects %}
  <article class="project">
    <div class="project-header">
      <h2 class="project-title"><a href="{{ project.url }}">{{ project.title }}</a></h2>
      <span class="project-date">{{ project.date | date: "%B %Y" }}</span>
    </div>
  </article>
  {% endfor %}
</div>
