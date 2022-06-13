---
title: "Projects"
layout: archive
permalink: /projects/
collection: archive
entries_layout: grid
classes: wide
date: 2020-11-03T18:38:52+00:00


---

These are the various projects that I have worked on for school, robotics, or during my free time for fun! 

<h2>Pages</h2>
{% for post in site.pages %}
  {% include archive-single.html %}
{% endfor %}
