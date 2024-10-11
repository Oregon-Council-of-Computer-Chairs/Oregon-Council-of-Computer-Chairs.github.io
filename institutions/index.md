---
title: Institutions
---

<ul id="institutions">
{% for i in site.institutions %}
    {% assign today_date = 'now' | date: '%s' %}
    {% assign max_age = 400 | times: 24 | times: 60 | times: 60 %}
    {% assign cutoff_date = today_date | minus: max_age %}
    {% assign last_update_string = i.last_update | date: '%s' %}
    {% assign last_update = last_update_string | plus: 0 %}

    {% if last_update > cutoff_date %}
    <a href="{{i.machine_name}}" alt="{{i.name}}">{{i.name}}</a>
    {% endif %}
{% endfor %}
</ul>
