---
title: Blog
in_sidebar: true
---
# Blog

<div>
{% for post in site.posts %}
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p><small>{{ post.date | date: "%-d %B %Y" }}</small></p>
    <p>{{ post.excerpt | strip_html }}</p>
    <hr>
{% endfor %}
{% if site.posts.size == 0%}
There doesn't seem to be anything here. Can I interest you in <a href="/">a home page</a>?
{% endif %}
</div>