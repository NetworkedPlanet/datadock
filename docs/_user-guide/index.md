---
title: User Guide
layout: page
order: 0
---

<ul list="toclist">
	{% assign ordered_docs = site.user-guide | sort: "order" %}
	{% for doc in ordered_docs %}
		{% if doc.order > 0 and doc.order < 100 %}
			<li><a href="{{ doc.url  | prepend: site.baseurl }}">{{doc.title}}</a></li>
		{%endif%}
	{% endfor %}
</ul>

<h2>In Detail</h2>

<ul list="toclist">
	{% assign ordered_docs = site.user-guide | sort: "order" %}
	{% for doc in ordered_docs %}
		{% if doc.order > 99 and doc.order < 201 %}
			<li><a href="{{ doc.url  | prepend: site.baseurl }}">{{doc.title}}</a></li>
		{%endif%}
	{% endfor %}
</ul>