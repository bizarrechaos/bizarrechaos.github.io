---
layout: default
permalink: /category/
---

<p>$ ls -l <span class="string">categories</span> | grep -e total -e '^d' | awk {'print $9, $5'}<br />total {{ site.tags | size }}</p>
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
            $ cat <span id="{{ category[0] }}" class="string">category[0]</span>
        <!--<ul class="post-list">
        {% assign list = category[1] %}
        {% for post in list %}
            <li>
                <a href="{{ post.url }}">{{ post.title }}</a>
            </li>
        {% endfor %}
        {% assign pages_list = nil %}
        {% assign group = nil %}
        </ul>-->
        {% endfor %}
    {% assign taglist = nil %}
</p>
