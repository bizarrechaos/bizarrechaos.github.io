---
layout: default
---
<p>ls -lt <a class="string" href="{{ site.url }}/posts/">posts</a><br />total {{ site.posts | size }}</p>
<p>
    {% for post in site.categories.posts %}
        -rw-r--r-- 1 bizarrechaos admin {{ post.content | size }} {{ post.date | date: "%b %d %Y %H:%M" }} <a class="string" href="{{ post.url }}">{{ post.title }}</a><br />
    {% endfor %}
</p>
