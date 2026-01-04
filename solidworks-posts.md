---
layout: default
title: "Posts from Solidworks"
permalink: /solidworks/
---

## Posts from Solidworks

<ul>
  {% for post in site.posts %}
    {% if post.path contains '_posts/solidworks/' %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <span> - {{ post.date | date: "%B %d, %Y" }}</span>
        <p>{{ post.excerpt }}</p>
      </li>
    {% endif %}
  {% endfor %}
</ul>
