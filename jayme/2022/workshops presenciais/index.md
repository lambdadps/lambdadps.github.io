---
title: Workshops
---
<h1>Workshops presenciais</h1>

 <table style="width:100%">
  <tr>
    <th>10h às 12h</th>
    <th>13h às 15h</th>
    <th>16h às 18h</th>
    <th>19h às 21h</th>
  </tr>
  <tr>
    <td>Curso 1</td>
    <td>Curso 2</td>
    <td>Curso 3</td>
    <td>Curso 4</td>
  </tr>
  <tr>
    <td>Curso 5</td>
    <td>Curso 6</td>
  </tr>
</table> 

{% for workshop in site.workshops %}
    {% if workshop.eventcode contains 'jayme4-presencial' %}
    <h2><a href="{{ workshop.url }}">{{ workshop.title }}</a></h2>
    <h4>{{ workshop.vagas }}</h4>
    <p><b>Ministrante:</b> {{ workshop.lecturer }}</p>
    <p><b>Horário:</b> {{ workshop.schedule }}</p>
    {% endif %}
{% endfor %}

<h1>Workshops à distância</h1>
