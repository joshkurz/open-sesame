---
layout: standard
title: "Atlanta Locksmith Blog"
slug: blog
permalink: /atlanta-locksmith-blog/
sitemap:
    priority: 1
    changefreq: 'monthly'
    lastmod: 2016-01-29T12:49:30-05:00
---

<div class="container">
    <h1>
        <a href="#" class="history-back"><i class="icon-arrow-left-3 fg-darker smaller"></i></a>
        Blog Posts
    </h1>
    <div class="listview-outlook postslist">
        {% for post in site.posts %}
        <a href="{{ site.baseurl }}{{ post.url }}" class="list">
            <div class="list-content">
                <div class="tile half">
                    <div>
                        {{ post.date | date: "%B" }}
                    </div>
                    <div>
                        {{ post.date | date: "%-d" }}
                    </div>
                    <div>
                        {{ post.date | date: "%Y" }}
                    </div>
                </div>
                <h2>{{ post.title }}</h2>
            </div>
        </a>
        {% endfor %}
    </div>
</div>
