---
title: Online Hosted Instructions
permalink: index.html
layout: home
---

# Microsoft Learn - Dialog Exercises

The following dialog exercises are designed to support [Microsoft Learn](https://docs.microsoft.com/training/) training.

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions'" %}
| |
| --- | --- | 
{% for activity in labs  %}| [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}
