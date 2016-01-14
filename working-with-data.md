---
layout: page
title: Animals
animals:
 - dog
 - sow
---

## All Animals

{% for animal in site.data.animals %}
**{{ animal.name }}** - {{ animal.desc | truncatewords: 6, '&hellip;' }}
{% endfor %}

---

## Some Animals
{% for page_animal in page.animals %}
  {% for animal in site.data.animals %}
    {% if page_animal == animal.name %}
**{{ animal.name }}** - {{ animal.desc | truncatewords: 6, '&hellip;' }}
    {% endif %}
  {% endfor %}
{% endfor %}

---

## One Animal

{% assign filtered_animals = site.data.animals | where:"name","crane" %}
{% for animal in filtered_animals %}
**{{ animal.name }}** - {{ animal.desc | truncatewords: 6, '&hellip;' }}
{% endfor %}

*OR*

{% assign animal = site.data.animals.[4] %}
**{{ animal.name }}** - {{ animal.desc | truncatewords: 6, '&hellip;' }}
