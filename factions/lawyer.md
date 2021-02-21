---
title: lawyer folx
faction: lawyers
---

{% assign faction = site.data.factions[page.faction] %}
The {% include faction_ping.html faction=page.faction %} are a [faction]({{ "/factions" | relative_url }}) within Amylandia.

{% include contrib_stub.md %}
