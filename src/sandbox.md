---
layout: page
title: Sandbox - for developing components
---

Insert a tune card component here:
{% render "tune_card", title: "Haste to the Wedding" %}


<ul>
  {% for post in collections.posts.resources %}
    <li>
      <a href="{{ post.relative_url }}">{{ post.data.title }}</a>
    </li>
  {% endfor %}
</ul>

If you have a lot of posts, you may want to consider adding [pagination](https://www.bridgetownrb.com/docs/content/pagination)!
