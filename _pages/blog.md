---
layout: archive
title: "Blog"
permalink: /blog/
author_profile: true
---

This is a space for me to share reflections on my research, and all things platforms, policy, social science, and tech writ large. I’ll also provide thoughts on academic life and the occasional musings on whatever else I find compelling to write about. Thanks for stopping by!

{% include base_path %}

{% assign posts = site.posts
  | where_exp: 'p', 'p.published != false'
  | where_exp: 'p', 'p.date <= site.time' %}

{% for post in posts %}
  {% include archive-single.html %}
{% endfor %}