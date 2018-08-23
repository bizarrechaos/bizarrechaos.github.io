---
layout: default
---
<p>ls -lt <a href="{{ site.url }}/posts/">posts</a><br />total {{ site.posts | size }}</p>
<ul class="posts">
    {% for post in site.posts %}
        <li>
            <a class="string" href="{{ post.url }}">{{ post.title }}</a>
        </li>
    {% endfor %}
</ul>
