---
layout: default
title: Main Page
---
The Soccer Coaching Odyssey
==========================

This site serves the purpose of sharing my development as a soccer coach. It is my hope that, in sharing this, others will benefit, as well as, provide me with useful feedback. The topics of posts range from training sessions to tactical theory to physiological and psychological development of youth players. Alongside the posts, I am creating my own guidebook that covers every aspect of coaching that I have touched upor so far. It will continually be added to and revised, but will always be available for you to download and draw from.

{% for post in site.posts limit: 10 %}
<div class="row">
    <div class="col-md-12">
        <h2>{{ post.title }}</h2>
        <h4>{{ post.date | date_to_long_string }}</h4>
        <p>
            <a href="{{ post.url }}">Read Post</a>
        </p>
    </div>
</div>
{% endfor %}
