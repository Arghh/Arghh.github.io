---
layout: blog
title: Blob
permalink: /blog/
---
{% for post in site.posts %}
{% include JB/post_content %}
{% endfor %}
and post_content

<article class="unit-article layout-post">
    <div class="unit-inner unit-article-inner">
        <div class="content">
            <div class="bd">
                <div class="entry-content">
                    {{ post.content }}
                </div><!-- entry-content -->
            </div><!-- bd -->
        </div><!-- content -->
    </div><!-- unit-inner -->
</article>
