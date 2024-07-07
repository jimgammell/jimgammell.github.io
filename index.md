---
layout: base
title: Home
---

# List of blogposts:

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    - <small>{{ post.date | date: "%B %d, %Y" }}</small>
  </li>
{% endfor %}
</ul>