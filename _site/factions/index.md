# Factions

There are many factions within Amylandia.

<ul>
{% for faction in site.data.factions %}
  <li>
    <a href="faction/{{faction[0]}}" style="color:{{faction[1].color}}">{{ faction[1].name }}</a>
    {% if faction[1].desc %}
      - {{ faction[1].desc }}
    {% endif %}

    {% if faction[1].subfactions %}
      <ul>
      {% for subfaction in faction[1].subfactions %}
        <li>
          <a href="faction/{{subfaction[0]}}" style="color:{{subfaction[1].color}}">{{ subfaction[1].name }}</a>
        {% if subfaction[1].desc %}
          - {{ subfaction[1].desc }}
        {% endif %}
        </li>
      {% endfor %}
      </ul>
    {% endif %}
  </li>
{% endfor %}
</ul>
