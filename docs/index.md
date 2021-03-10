---
layout: page
---

# Home page

Check out this <a href="{{site.baseurl}}/math-demo.html"> page with math</a>!
It is way more interesting. 

Also, this is how you [create github pages manually][1].

<hr>

## Posts
{% for post in site.posts %}
<div class="post-preview">
    <a href="{{ post.url | prepend: site.baseurl }}">
        &raquo; {{ post.title }}
        {% if post.subtitle %}
        &mdash;
        {{ post.subtitle }}
        {% endif %}
    </a>
    <p class="post-meta" style="font-size: 16px">
       Posted on {{ post.date | date: "%-d %b, %Y" }}
    </p>
</div>
{% endfor %}


[1]: https://help.github.com/articles/creating-project-pages-manually
