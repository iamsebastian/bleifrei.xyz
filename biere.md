---
layout: inner
title: Biere
permalink: /biere/
---

# Biere, Sude, Gebrautes

> Keinen müden Tropfen, haben wir bisher vermaischt. Keinen. Auch nicht nur einen.

Zumindest ist dies das, was neulich noch hier stand. Mittlerweile gibt es etwas mehr:

{% for beer in site.data.beer %}
  {% if beer[1].brewed %}
  - [ **({{ beer[0] }}) {{ beer[1].name }}** ]( ../{{beer[0]}}/ )
  {% else %}
  - [ ({{ beer[0] }}) {{ beer[1].name }} ]( ../{{beer[0]}}/ )
  {% endif %}
{% endfor %}
