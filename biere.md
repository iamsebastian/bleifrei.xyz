---
layout: inner
title: Biere
permalink: /biere/
---

# Biere, Sude, Gebrautes

> Keinen müden Tropfen, haben wir bisher vermaischt. Keinen. Auch nicht nur einen.

Zumindest ist dies das, was neulich noch hier stand. Mittlerweile gibt es etwas mehr:

{% for beer in site.data.beer %}
  - [ ({{ beer[0] }}) {{ beer[1].name }} ]( ../{{beer[0]}}/ )
{% endfor %}
