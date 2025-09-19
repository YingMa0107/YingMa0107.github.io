---
layout: default
title: "Publications"
permalink: /publications/
---

{% assign groups = site.data.publish | sort: 'year' | reverse %}

## Publications

{% for g in groups %}
### {{ g.year }}
<ul class="pub-list">
  {% for it in g.items %}
    <li>{{ it.cite | markdownify | remove: '<p>' | remove: '</p>' }}</li>
  {% endfor %}
</ul>
{% endfor %}

<hr>

<div class="pub-legend">
  <span><code>*</code> co-first author</span> ·
  <span><code>†</code> co-corresponding author</span> ·
  <span><code>+</code> corresponding author</span>
</div>
