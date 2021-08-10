---
title: Standards
slug: index
type: index
---

{% assign standards = site.pages | where:'type','standard' | sort:"name" %}
<ul>
{% for standard in standards %}
<h2>{{ standard.title }}</h2>
  <li>{{ standard.sub_categories }}</li> 
  <li>{{ standard.date_initiated }}</li>
  <li>{{ standard.founded_by }}</li>
  <li>{{ standard.current_url }}</li>
  <li>{{ standard.goals }}</li>
  <li>{{ standard.status}}</li>
{% endfor %}
<ul>
