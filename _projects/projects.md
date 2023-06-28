---
title: "Projects"
layout: archive
permalink: /projects/
collection: archive
entries_layout: grid
classes: wide
date: 2022-06-13T18:38:52+00:00


---

This page is a list of my various projects that I have worked on for fun! The list includes projects for school, robotics, hobbies, and work.

<h2>Pages</h2>
{% for post in site.pages %}
  {% include archive-single.html %}
{% endfor %}
