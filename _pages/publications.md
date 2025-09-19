---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
{% assign groups = site.data.publish | sort: 'year' | reverse %}

<nav class="years-nav" style="margin-bottom:1rem;">
  {% for g in groups %}
    <a href="#y{{ g.year }}" style="margin-right:0.5rem;">{{ g.year }}</a>
  {% endfor %}
</nav>

{% for g in groups %}
### <a id="y{{ g.year }}"></a>{{ g.year }}

<ul class="pub-list">
  {% for it in g.items %}
    <li class="pub-item">
      {{ it.cite | markdownify | remove: '<p>' | remove: '</p>' }}
    </li>
  {% endfor %}
</ul>
{% endfor %}
