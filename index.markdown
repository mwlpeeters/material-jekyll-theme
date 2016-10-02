---
layout: page
title: Material Jekyll Theme
---



{% for post in site.posts | limit:3   %}
{% if forloop.first %}
<section>
<h2 class="c-archives__main" id="{{ this_year }}-ref">Latest articles</h2>
<ul class="c-archives__list">
    {% endif %}
    <li>
        <article role="article" class="c-archives__item">
            <h3><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
            <p>{{ post.description}} - {{ post.date | date: "%b %-d, %Y" }}</p>
        </article>
    </li>
    {% if forloop.last %}
</ul>
</section>
{% endif %}
{% endfor %}