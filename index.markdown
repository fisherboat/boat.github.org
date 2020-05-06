---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
permalink: /
layout: default
title: 最新博文
---

<div class="row mb-5">
  {% for post in site.categories["最新"] %}
    <div class="col-md-4">
      <div class="card">
        <div class="card-body">
          <h5 class="card-title"><a href="{{ post.url }}">{{post.title}}</a></h5>
          <p class="card-text">{{post.summary | truncatewords: 10, '...' }}</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>