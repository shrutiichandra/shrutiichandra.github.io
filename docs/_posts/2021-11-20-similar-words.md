---
layout: post
title:  "Similar words in Spanish & Italian"
categories: jekyll update
---
<table>
  {% for row in site.data.common %}
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
