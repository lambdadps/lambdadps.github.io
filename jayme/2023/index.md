---
title: Workshops
---
<h1>Workshops</h1>

 <table style="width:100%">
  <tr>
    <th> - </th>
    <th> - </th>
    <th> - </th>
    <th> - </th>
  </tr>
  <tr>
    <td> - </td>
    <td> - </td>
    <td> - </td>
    <td> - </td>
  </tr>
  <tr>
    <td> - </td>
    <td> - </td>
    <td> - </td>
    <td> - </td>
  </tr>
  <tr>
    <td></td>
    <td> - </td>
    <td> - </td>
    <td></td>
  </tr>
</table> 

{% for workshop in site.workshops %}
    {% if workshop.eventcode contains 'jayme5' %}
    <h2><a href="{{ workshop.url }}">{{ workshop.title }}</a></h2>
    <h4>{{ workshop.vagas }}</h4>
    <p><b>Ministrante:</b> {{ workshop.lecturer }}</p>
    <p><b>Horário:</b> {{ workshop.schedule }}</p>
    {% endif %}
{% endfor %}
