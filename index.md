---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Content Directory

Hyperlinks to each case study is listed below.

## Case Studies

{% assign casestudy = site.pages | where_exp:"page", "page.url contains '/Instructions/CaseStudy'" %}
| Module | Case Study |
| --- | --- | 
{% for activity in casestudy  %}| {{ activity.casestudy.module }} | [{{ activity.casestudy.title }}{% if activity.casestudy.type %} - {{ activity.casestudy.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
