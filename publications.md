---
layout: page
title: Publications
permalink: /publications/
---

{% for annual in site.data.publications %}
<h2>{{ annual.year }}</h2>
<ul>
{% for publication in annual.publications %}
<li>
<div><a href="{{publication.link}}">{{ publication.title }}</a></div>
<div style="font-size: 0.8em; font-style: italic">{{ publication.authors }}</div>
<div style="font-size: 0.8em; font-weight: 500">{{ publication.venue }}</div>
</li><br>
{% endfor %}
</ul>
{% endfor %}

