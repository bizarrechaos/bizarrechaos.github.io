---
layout: default
permalink: /category/
---

<p>$ ls -l /categories/*/ | grep -e total -e '^d' | awk {'print $9, $5'}<br />total {{ site.tags | size }}</p>
<p>
    {% assign list = site.tags | sort %}
        {% for category in list %}
            <a href="#{{ category[0] }}">{{ category[0] }}</a>&nbsp;{{ category[1].size }}<br />
        {% endfor %}
    {% assign list = nil %}
</p>

{% assign taglist = site.tags | sort %}
{% for category in taglist %}
 <h2 id="{{ category[0] }}">{{ category[0] }}</h2>
 <ul class="post-list">
  {% assign list = category[1] %}
  {% for post in list %}
   <li>
   <a href="{{ post.url }}">{{ post.title }}</a>
   </li>
  {% endfor %}
  {% assign pages_list = nil %}
  {% assign group = nil %}
 </ul>
{% endfor %}
{% assign taglist = nil %}
