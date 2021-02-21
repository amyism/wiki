---
title: happy fellows
faction: happy_fellow
---

{% assign faction = site.data.factions[page.faction] %}
# {{ faction.name }}

{% include stub.md %}

The {% include faction_ping.html faction=page.faction %} are a [faction]({{ "/factions" | relative_url }}) within Amylandia.
