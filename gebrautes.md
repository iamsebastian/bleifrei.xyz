---
layout: inner
title: Gebrautes
permalink: /gebrautes/
---

# Gebrautes

Keinen müden Tropfen, haben wir bisher vermaischt. Keinen. Auch nicht nur einen.

<ul>
{% for beer in site.data.beer %}
  <li><a href="../{{beer[0]}}/">({{ beer[0] }}) {{ beer[1].name }}</a></li>
{% endfor %}
</ul>
