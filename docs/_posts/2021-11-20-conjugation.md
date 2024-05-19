---
layout: post
title:  "Conjugation"
categories: jekyll update
---
<ul>
   {% for item in site.data.conjugationnav.docs %}
      <li><a href="{{ item.url }}">{{ item.title }}</a></li>
   {% endfor %}
</ul>
