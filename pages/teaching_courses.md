---
title: Courses Taught
layout: page
permalink: /teaching/courselist/
group: teaching
---

## Courses Taught

{% assign courses_grouped = site.data.courses | group_by: 'coursegroup' | sort: 'coursesemesterid' %}
{% for group in courses_grouped %}

### {{group.name}}

<table class="stack">
  <thead>
    <tr>
      <th>Semester</th>
      <th>Format</th>
      <th>Assignments</th>
    </tr>
  </thead>
  <tbody>
{% for item in group.items %}
    <tr>
      <td data-label="Semester">{% if item.courseid.size > 1 %}<a href="/courses/{{item.courseid}}">{% endif %}{{item.coursesemester}}{% if item.courseid.size > 1 %}</a>{% endif %}</td>
      <td data-label="Format">{% if group.name == "Digital History for Undergraduates" or  group.name == "Medieval Survey" %}{{item.course}}: {% endif %}{{item.coursetype}}</td>
      <td data-label="Short Desc">{{item.coursegrading}}</td>
    </tr>
{% endfor %}
  </tbody>
</table>
{% endfor %}

