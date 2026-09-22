---
layout: default
title: 카테고리
permalink: /categories/
---
<section class="shell standard-page category-index">
  <p class="eyebrow">주제별 탐색</p>
  <h1>카테고리<span class="heading-period">.</span></h1>
  <p class="page-lead">관심 있는 주제를 선택해 글을 살펴보세요.</p>
  <div class="category-grid">
    {% for category in site.data.categories %}
    {% assign category_posts = site.posts | where: 'category', category.id %}
    <a class="category-card" href="{{ category.url | relative_url }}">
      <span class="category-card-top"><span>0{{ forloop.index }}</span><span aria-hidden="true">↗</span></span>
      <strong>{{ category.name }}</strong>
      <span class="category-description">{{ category.description }}</span>
      <span class="category-count">글 {{ category_posts.size }}개</span>
    </a>
    {% endfor %}
  </div>
</section>
