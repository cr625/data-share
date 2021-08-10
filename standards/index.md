---
title: Standards
slug: index
type: index
---

{% assign standards = site.pages | where:'type','standard' | sort:"name" %}
{% for standard in standards %}
{{ standard.title }}
{% endfor %}
