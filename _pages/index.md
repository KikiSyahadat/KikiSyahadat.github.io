---
layout: defaults/page
permalink: index.html
narrow: true
title: Selamat Datang!
---

{% include components/intro.md %} [Caranya bisa dibaca](about.html#buy-me-coffee) [di halaman Tentang](about.html).

---

### Tulisan Terbaru

{% for post in site.posts limit:3 %}
{% include components/post-card.html %}
{% endfor %}

### [Semua Tulisan](list/posts.html)

---

