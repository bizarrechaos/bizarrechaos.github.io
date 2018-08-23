---
layout: content
---
ls -lt <a href="{% site.url %}/posts/">posts</a>
total {% site.posts | size %}
<ul class="posts">
    {% for post in site.posts %}
        <li>
            <a class="reserved" href="{{ post.url }}">{{ post.title }}</a>
        </li>
    {% endfor %}
</ul>
