---
layout: page
---

# Home page

Check out this <a href="{{site.baseurl}}/math-demo.html"> page with math</a>!
It is way more interesting. 

<hr>

## Posts
{% for post in site.posts %}
<div class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
        &raquo; {{ post.title }}
        {% if post.subtitle %}
        &mdash;
        <a class="post-subtitle">
            {{ post.subtitle }}
        </a>
        {% endif %}
    </a>
    <p class="post-meta" style="font-size: 16px">
       Posted on {{ post.date | date: "%-d %b, %Y" }}
    </p>
</div>
{% endfor %}


