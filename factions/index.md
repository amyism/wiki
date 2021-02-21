# Factions

There are many factions within Amylandia.

2

<ul>
{% for faction in site.data.factions %}
  <li>
    {% assign faction_id = faction[0] %}
    {% include faction_ping.html faction=faction_id %}

    {% if faction[1].desc %}
      - {{ faction[1].desc }}
    {% endif %}
  </li>
{% endfor %}
</ul>

{% include contrib_stub.md %}
