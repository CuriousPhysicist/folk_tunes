---
layout: page
title: Sandbox - for developing components
---

## Things to do:
* Get a MusicXML file to render in a component
    * incorporate OSMD library into the website
* find or create MusicXML files for all the tunes

Insert tune card components here:
{% for tune in site.data.tunes %}
{% render "tune_card", title: tune %}
{% endfor %}



<ul>
  {% for post in collections.posts.resources %}
    <li>
      <a href="{{ post.relative_url }}">{{ post.data.title }}</a>
    </li>
  {% endfor %}
</ul>

If you have a lot of posts, you may want to consider adding [pagination](https://www.bridgetownrb.com/docs/content/pagination)!
