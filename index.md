---
layout: content
---
<div class="row">
    <div class="col-lg-8 col-lg-offset-2">
        <p>ls -lt <a href="{{ site.url }}/posts/">posts</a><br />total {{ site.posts | size }}</p>
        <ul class="posts">
            {% for post in site.posts %}
                <li>
                    <a class="reserved" href="{{ post.url }}">{{ post.title }}</a>
                </li>
            {% endfor %}
        </ul>
    </div>
</div>
