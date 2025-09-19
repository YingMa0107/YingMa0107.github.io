---
layout: default
title: "Publications"
permalink: /publications/
---

<h1>Publications</h1>

{% assign groups = site.data.pubs_by_year | sort: 'year' | reverse %}
{% for g in groups %}
  <h2>{{ g.year }}</h2>
  <ul class="pub-list">
    {% for it in g.items %}
      <li>{{ it.cite | markdownify | remove: '<p>' | remove: '</p>' }}</li>
    {% endfor %}
  </ul>
{% endfor %}

<hr/>

<p><sub>
* `*` denotes <strong>co-first author</strong>.<br/>
* `†` denotes <strong>co-corresponding author</strong>.<br/>
* `+` denotes <strong>corresponding author</strong>.
</sub></p>
