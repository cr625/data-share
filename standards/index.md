---
title: Standards
slug: index
type: index
---

{% assign standards = site.pages | where:'type','standard' | sort:"name" %}
{% for standard in standards %}
{{ standard.title }}
{{ sub_categories }}
{{ date_initiated }}
{{ founded_by }}
{{ current_url }}
{{ goals }}
{{ status}}
{% endfor %}
