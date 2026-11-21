---
layout: default
title: Blog
permalink: /blog/
---

# Blog

{% if site.posts.size == 0 %}
No posts yet.
{% endif %}
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) - *{{ post.date | date_to_string }}*
{% endfor %}
