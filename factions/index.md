# Factions

There are many factions within Amylandia.

1

<ul>
{% for faction in site.data.factions %}
  <li>
    {% capture faction_id %}{{ faction[0] }}{% endcapture %}
    {% include faction_ping.html faction=faction_id %}


    {% if faction[1].desc %}
      - {{ faction[1].desc }}
    {% endif %}
  </li>
{% endfor %}
</ul>

{% include contrib_stub.md %}
