---
layout: archive
title: "News"
permalink: /news/
author_profile: true
---
## &#x1F4E3; News

{% assign newsItems = site.data.news %}
{% for news in newsItems %}
{{ news.date | date: "%B %d, %Y" }}: {{ news.title }}
{% endfor %}

