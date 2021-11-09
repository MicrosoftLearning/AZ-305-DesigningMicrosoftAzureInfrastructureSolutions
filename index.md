---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Hyperlinks to each case study is listed below.

## Case Studies

{% assign CaseStudy = site.pages | where_exp:"page", "page.url contains '/Instructions/Case Study'" %}
| Module | CaseStudy |
| --- | --- | 
{% for activity in CaseStudy %}| {{ activity.CaseStudy.module }} | [{{ activity.CaseStudy.title }}{% if activity.CaseStudy.type %} - {{ activity.CaseStudy.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

