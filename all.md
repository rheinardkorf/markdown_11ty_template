---
title: All Posts
seoDescription: All posts on my site.
---

{% for post in collections.allThings %}
[[{{post.data.title}}]]  
{% endfor %}

<!-- [//begin]: -->
{% for post in collections.allThings %}
[{{post.data.title}}]: {{post.url | remove: "/" }} "{{post.data.title}}"
{% endfor %}
<!-- [//end]: -->
