---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Welcome to my blog.

<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    - <small>{{ post.date | date: "%B %d, %Y" }}</small>
  </li>
{% endfor %}
</ul>