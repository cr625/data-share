---
title: Standards
slug: index
type: index
---

{% assign standards = site.pages | where:'type','standard' | sort:"name" %}
<dl>
{% for standard in standards %}
<h2>{{ standard.title }}</h2>
  <dt>Sub-categories</dt>
  <dd>{{ standard.sub_categories }}</dd> 
  
  <dt>Date Initiated</dt>
  <dd>{{ standard.date_initiated }}</dd>
  
  <dt>Founded by</dt>
  <dd>{{ standard.founded_by }}</dd>
  
  <dt>Current URL</dt>
  <dd>{{ standard.current_url }}</dd>
  
  <dt>Goals</dt>
  <dd>{{ standard.goals }}</dd>
  
  <dt>Status</dt>
  <dd>{{ standard.status}}</dd>
{% endfor %}
<dl>
