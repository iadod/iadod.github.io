---
layout: page
title: Projects
permalink: /projects/
---

As a complement to my [primary work experience](https://iadod.github.io/resume/), the following are some projects I've worked on, including side quests.

{% for project in site.categories.projects reversed %}
  <div style="margin-bottom: 2rem;">
    <h2><a href="{{ project.url }}">{{ project.title }}</a></h2>
  </div>
{% endfor %}
