---
layout: default
ref: lavr-2022
lang: ru
title: Лаврентьевские чтения 2022
---
# Лаврентьевские чтения 2022

## Личный зачёт

<table>
  <thead>
    <tr>
      <th>Участник</th>
      <th>Команда</th>
      <th>Статус</th>
      <th>A</th>
      <th>B</th>
      <th>C</th>
      <th>D</th>
      <th>E</th>
      <th>Всего</th>
    </tr>
  </thead>
  <tbody>
    {% for res in site.data.lavr.pers22.results -%}
    <tr>
      <td>{{ res.surname }} {{ res.name }} {{ res.patronymic }}</td>
      <td>{{ res.team }}</td>
      <td>{{ res.status }}</td>
      <td class="right">{{ res.problems[0] }}</td>
      <td class="right">{{ res.problems[1] }}</td>
      <td class="right">{{ res.problems[2] }}</td>
      <td class="right">{{ res.problems[3] }}</td>
      <td class="right">{{ res.problems[4] }}</td>
      <td class="center">{{ res.total }}</td>
    </tr>
    {%- endfor %}
  </tbody>
</table>

## Командный зачёт

<table class="table table-bordered">
  <thead>
    <tr>
      <th>Команда</th>
      <th>Комментарий</th>
      <th>Всего</th>
    </tr>
  </thead>
  <tbody>
    {% for res in site.data.lavr.team22.results -%}
    <tr>
      <td>{{ res.team }}</td>
      <td>{{ res.comment }}</td>
      <td class="center">{{ res.total }}</td>
    </tr>
    {%- endfor %}
  </tbody>
</table>
