---
layout: archive
title: "News"
permalink: /news/
author_profile: true
---
## &#x1F4E3; News
<div style="text-align:justify">
{% assign newsItems = site.data.news | sort: 'date' | reverse %}
{% for news in newsItems %}
{{ news.date | date: "%B %d, %Y" }}: {{ news.title | markdownify | replace: '<p>', '' | replace: '</p>', '' }}
{% endfor %}
</div>


