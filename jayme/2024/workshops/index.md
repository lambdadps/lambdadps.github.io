---
title: Workshops
---
<h1>Cursos</h1>

 <table style="width:100%">
  <tr>
    <th> horario 1 </th>
    <th> horario 2 </th>
    <th> horario 3 </th>
  </tr>
  <tr>
    <td> curso h1 </td>
    <td> curso h2 </td>
    <td> curso h3 </td>
  </tr>
  <tr>
    <td> curso h1 </td>
    <td> curso h2 </td>
    <td> curso h3  </td>
  </tr>
  <tr>
    <td>  </td>
    <td> curso h2 </td>
   <td>  </td>
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

