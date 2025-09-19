---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
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

---

<sub>
* `*` denotes **co-first author**.  
* `†` denotes **co-corresponding author**.  
* `+` denotes **corresponding author**.  
</sub>
