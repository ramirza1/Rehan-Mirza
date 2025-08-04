---
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

<ul>
  <li><a href="{{ '/about/' | relative_url }}">About</a></li>
  <li><a href="{{ '/research/' | relative_url }}">Research & Projects</a></li>
  <li><a href="{{ '/cv/' | relative_url }}">CV</a></li>
  <li><a href="{{ '/phd-guidance/' | relative_url }}">Advice for PhD Applicants</a></li>
  <li>
    <a href="{{ '/blog/' | relative_url }}">Blog</a>
    {% assign posts = site.posts | where_exp: 'p', 'p.published != false' %}
    {% if posts.size > 0 %}
      <ul>
        {% for post in posts limit:5 %}
          <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
        {% endfor %}
      </ul>
    {% endif %}
  </li>
</ul>