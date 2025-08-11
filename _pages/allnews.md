---
title: "News"
layout: textlay
excerpt: "Allan Lab at Leiden University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p><strong>{{ article.date }}</strong><br>{{ article.headline }}</p>
{% endfor %}
