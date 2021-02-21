# Factions

There are many factions within Amylandia.

<ul>
{% for faction in site.data.factions %}
  <li>
    {% include faction_ping.html faction="faction[0]" %}
    {% if faction[1].desc %}
      - {{ faction[1].desc }}
    {% endif %}
  </li>
{% endfor %}
</ul>

{% include contrib_stub.md %}
