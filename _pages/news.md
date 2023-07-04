---
layout: page
title: News
permalink: /news/
---

## :mega: Latest News
{% for news in site.data.news %}
### {{ news.date }}: {{ news.title }}

{{ news.description }}

{% endfor %}