---
layout: default
permalink: /posts/
---

<p>$ ls -lt <span class="string">posts</span><br />total {{ site.posts | size }}</p>
<p>
    {% for post in site.categories.posts %}
        -rw-r--r-- 1 {{ site.nick }} admin {{ post.content | size }} {{ post.date | date: "%b %d %Y %H:%M" }} <a class="string" href="{{ post.url }}">{{ post.title }}</a><br />
    {% endfor %}
</p>
