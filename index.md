---
title: Home
layout: page
---
<div class="page-title" id="latest-posts">Latest Posts</div>
<div class="archive-main">
  {% for post in site.posts limit:10 %}
    <div class="archive-item">
      <div class="archive-date">{{ post.date | date:"%B %d, %Y" }}</div>
      <div class="archive-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></div>
    </div>
  {% endfor %}
</div>
<p class="archive-more">
  <a href="{{ "pages/archive.html" | relative_url }}">More</a> |
  <a href="{{ "/feed.xml" | relative_url }}">Subscribe</a>
</p>
