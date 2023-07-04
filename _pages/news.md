---
layout: archive
title: "News"
permalink: /news/
author_profile: true
---

## &#x1F4E3; News
{% for news in site.data.news %}
### {{ news.date }}: {{ news.title }}

{{ news.description }}

{% endfor %}