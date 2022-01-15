---
layout: post
title:  "Conjugation"
date:   2021-11-20 10:29:00 +0530
categories: jekyll update
---
<table>
  {% for row in site.data.verbs %}
    {% if forloop.first %}
    <tr>
      {% for pair in row %}
        <th>{{ pair[0] }}</th>
      {% endfor %}
    </tr>
    {% endif %}

    {% tablerow pair in row %}
      {{ pair[1] }}
    {% endtablerow %}
  {% endfor %}
</table>