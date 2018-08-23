---
layout: default
---
<p>ls -lt <a href="{{ site.url }}/posts/">posts</a><br />total {{ site.posts | size }}</p>
<p>
    {% for post in site.posts %}
        <a class="string" href="{{ post.url }}">{{ post.title }}</a><br />
    {% endfor %}
</p>
