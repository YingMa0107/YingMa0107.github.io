---
layout: default
title: News
---

# News

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
<span>{{ post.date | date_to_string }}</span>

{{ post.content }}

[Back to News](index.md)
{% endfor %}