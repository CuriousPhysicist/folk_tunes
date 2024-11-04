---
layout: page
title: Sandbox - for developing components
---

## Things to do:
* Get a MusicXML file to render in a component
    * incorporate OSMD library into the website
* find or create MusicXML files for all the tunes

```
Put music here
```

<div id="osmdContainer"/>
<!-- script src="opensheetmusicdisplay.min.js"></script -->
<script src="https://unpkg.com/opensheetmusicdisplay@0.8.3/build/opensheetmusicdisplay.min.js">
<script>
  var osmd = new opensheetmusicdisplay.OpenSheetMusicDisplay("osmdContainer");
  osmd.setOptions({
    backend: "svg",
    drawTitle: true,
    // drawingParameters: "compacttight" // don't display title, composer etc., smaller margins
  });
  osmd
    .load("http://downloads2.makemusic.com/musicxml/MozaVeilSample.xml")
    .then(
      function() {
        osmd.render();
      }
    );
</script>

This are the Tune pages:


{% for tune in collections.tunes.resources %}
<a href="{{tune.relative_url}}">{{ tune.title }}</a>
{% endfor %}

