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

This is the Tune page:

{% assign my_resource = collections.tunes.resources.first %}
{{ my_resource.relative_url }}

{% for tune in collections.tunes.resources %}
  <h2>{{ tune.title }}</h2>
  <p>{{ tune.content | markdownify }}</p>
{% endfor %}

