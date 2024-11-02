---
layout: page
title: Tunes
---

Here are the current tunes I know:

<div class="card_box">
{% for tune in site.data.tunes %}
{% render "tune_card", title: tune %}
{% endfor %}
</div>

* Haste to the Wedding - Jig, Irish
* Lark in the Morning - Jig, Irish
* The Kesh Jig - Jig, Irish
* The Swallowtail Jig - Jig, Irish
* The Irish Washerwoman - Jig, Irish
* Old Tom of Oxford - Slow Air, English
* British Grenadiers - March, English
* The Sportsman's Hornpipe - Hornpipe, English
