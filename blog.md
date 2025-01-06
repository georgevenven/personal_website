---
layout: default
title: blog
---

# Blog Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) - *{{ post.date | date_to_string }}*
{% endfor %}