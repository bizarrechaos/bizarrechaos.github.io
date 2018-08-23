---
layout: content
---

<ul class="posts">
    {% for post in site.posts %}
        <li>
            <a class="reserved" href="{{ post.url }}">{{ post.title }}</a>
        </li>
    {% endfor %}
</ul>
