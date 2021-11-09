---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Hyperlinks to each case study is listed below.

## Case Studies

{% assign Case Studies = site.pages | where_exp:"page", "page.url contains '/Instructions/Case Study'" %}
| Module | Case Study |
| --- | --- | 
{% for activity in Case Study %}| {{ activity.Case Study.module }} | [{{ activity.Case Study.title }}{% if activity.Case Study.type %} - {{ activity.Case Study.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

