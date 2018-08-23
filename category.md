---
layout: default
permalink: /category/
---

<p>$ ls <span class="reserved">-l</span> <span class="string">categories</span> | grep <span class="reserved">-e</span> <span class="string">'total'</span> <span class="reserved">-e</span> <span class="string">'^d'</span> | awk <span class="string">'{print $9, $5}'</span><br />total {{ site.tags | size }}</p>
<p>
    {% assign list = site.tags | sort %}
    {% for category in list %}
        <a class="string" href="#{{ category[0] }}">{{ category[0] }}</a> {{ category[1].size }}<br />
    {% endfor %}
    {% assign list = nil %}
</p>
<p>
    {% assign taglist = site.tags | sort %}
    {% for category in taglist %}
        $ cat <span id="{{ category[0] }}" class="string">{{ category[0] }}</span><br />
        {% assign list = category[1] %}
        {% for post in list %}
            <a class="string" href="{{ post.url }}">{{ post.title }}</a><br />
        {% endfor %}
        <br />
        {% assign pages_list = nil %}
        {% assign group = nil %}
    {% endfor %}
    {% assign taglist = nil %}
</p>
