---
layout: defaults/page
permalink: index.html
narrow: true
title: Selamat Datang!
---

{% include components/intro.md %}

[Caranya bisa dibaca di sini.]({{ site.baseurl }}{% link about.md %})

<hr />

### Tulisan Terbaru

{% for post in site.posts limit:3 %}
{% include components/post-card.html %}
{% endfor %}


