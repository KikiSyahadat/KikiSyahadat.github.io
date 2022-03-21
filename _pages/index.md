---
layout: defaults/page
permalink: index.html
narrow: true
title: Selamat Datang!
---

{% include components/intro.md %}

---

### Tulisan Terbaru

{% for post in site.posts limit:3 %}
{% include components/post-card.html %}
{% endfor %}

#### [Lihat semua tulisan >>](list/posts.html)


