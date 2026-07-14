---
title: "ニュース"
permalink: /news/
excerpt: "プロジェクトの最新の進捗・お知らせ"
author_profile: true
---

プロジェクトの進捗やお知らせを掲載します。

{% if site.posts.size == 0 %}
現在、掲載されているニュースはありません。
{% else %}
{% assign postsByYear = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}
{% for year in postsByYear %}

## {{ year.name }}年

<ul class="news-list">
{% for post in year.items %}
  <li>
    <span class="news-date">{{ post.date | date: "%Y.%m.%d" }}</span>
    {% if post.categories.size > 0 %}<span class="news-cat">{{ post.categories | first }}</span>{% endif %}
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>
{% endfor %}
{% endif %}
