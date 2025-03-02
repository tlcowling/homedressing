---
layout: default
title: Blog
permalink: /blog/
---

<h1>Blog</h1>
<div class="blog-container">
    <div class="blog-content">
        <div class="blog-list">
            {% for post in site.posts %}
            <article class="blog-item">
                <div class="blog-thumbnail">
                    <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
                </div>
                <div class="blog-text">
                    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
                    <p class="blog-meta">Published on {{ post.date | date: "%B %d, %Y" }}</p>
                    <p>{{ post.content | strip_html | truncatewords: 30 }}</p>
                    <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
                </div>
            </article>
            {% endfor %}
        </div>
    </div>
    <aside class="blog-sidebar">
        <h2>Favorites</h2>
        <hr>
        <h2>Recent posts</h2>
        <hr>
        <ul>
            {% for post in site.posts limit:4 %}
            <li>
                <a href="{{ post.url | relative_url }}">
                    <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" class="sidebar-thumbnail">
                    {{ post.title }}
                </a>
            </li>
            {% endfor %}
        </ul>
    </aside>
</div>

