---
title: Standards
slug: index
type: index
---

{% assign standards = site.pages | where:'type','standard' | sort:"name" %}
{% for standard in standards %}
{{ standard.title }}
{{ standard.sub_categories }}
{{ standard.date_initiated }}
{{ standard.founded_by }}
{{ standard.current_url }}
{{ standard.goals }}
{{ standard.status}}
{% endfor %}
