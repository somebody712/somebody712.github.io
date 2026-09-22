---
layout: default
title: 글 목록
permalink: /archive/
---
<section class="shell standard-page">
  <p class="eyebrow">아카이브</p>
  <h1>글 목록<span class="heading-period">.</span></h1>
  <p class="page-lead">지금까지 남긴 기록을 한곳에서 볼 수 있습니다.</p>
  {% if site.posts.size > 0 %}
  <div class="archive-list">
    {% for post in site.posts %}
    {% assign post_category = site.data.categories | where: 'id', post.category | first %}
    <article class="archive-item">
      <div class="archive-meta"><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: '%Y. %m. %d.' }}</time><span>{{ post_category.name | default: '기록' }}</span></div>
      <h2><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h2>
      <span aria-hidden="true">↗</span>
    </article>
    {% endfor %}
  </div>
  {% else %}
  <p class="empty-message">아직 글이 없습니다.</p>
  {% endif %}
</section>
