---
layout: page
title: Projects
permalink: /projects/
---

<p>Main, Side Proj and Side Quests</p>

{% for project in site.categories.projects reversed %}
  <div style="margin-bottom: 2rem;">
    <h2><a href="{{ project.url }}">{{ project.title }}</a></h2>
  </div>
{% endfor %}
