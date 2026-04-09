---
layout: page
title: Projects
permalink: /projects/
---

<p>As a complement to the primary work experience described in my resume, the following are some of the projects I've worked on, including some side quests. </p>

{% for project in site.categories.projects reversed %}
  <div style="margin-bottom: 2rem;">
    <h2><a href="{{ project.url }}">{{ project.title }}</a></h2>
  </div>
{% endfor %}
