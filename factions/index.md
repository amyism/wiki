# Factions

There are many factions within Amylandia.

<ul>
{% for faction in site.data.factions %}
  <li>
    <span style="color:{{faction[1].color}}"><a href="faction/{{faction[0]}}">{{ faction[1].name }}</a></span>
    {% if faction[1].desc %}
      - {{ faction[1].desc }}
    {% endif %}

    {% if faction[1].subfactions %}
      <ul>
      {% for subfaction in faction[1].subfactions %}
        <li>
        <span style="color:{{subfaction[1].color}}"><a href="faction/{{subfaction[0]}}">{{ subfaction[1].name }}</a></span>
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
