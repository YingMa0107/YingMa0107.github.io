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
<p>{{ news.date | date: "%Y-%m-%d" }}: <strong>{{ news.title | replace: news.journal, '**' | replace: ': ', ':&nbsp;' | markdownify }}</strong></p>
{% endfor %}
</div>


