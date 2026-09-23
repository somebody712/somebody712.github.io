---
layout: default
title: 카테고리
permalink: /categories/
---
<section class="page-title"><h1>카테고리</h1><p>분야별 기록</p></section>
<div class="category-grid category-index">
  {% for item in site.data.categories %}{% assign matched = site.posts | where: 'category_slug', item.slug %}<a class="category-card" href="{{ '/categories/' | append: item.slug | append: '/' | relative_url }}"><span class="number">0{{ forloop.index }}</span><strong>{{ item.name }}</strong><span>글 {{ matched.size }}개</span></a>{% endfor %}
</div>
