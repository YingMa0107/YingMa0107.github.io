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
  <p>
    {{ news.date | date: "%Y-%m-%d" }}:
    {{ news.title | markdownify | remove: '<p>' | remove: '</p>' }}
  </p>
{% endfor %}
</div>


