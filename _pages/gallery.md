---
title: "Gallery"
layout: single
permalink: /gallery/
---

{% for author in site.data.authors %}
{% assign member = author[1] %}
{% if member.member %}
{% if member.current %}

## {{ gallery.name }}

{% if member.avatar %}
![Photograph of {{member.name}}]({{member.avatar}}){:style="float: left; object-fit: contain; width: 30%; max-height: 12em; margin-left: 1em; margin-right: 1em;"}
{% endif %}

{% if member.bio %}
**{{ gallery.bio }}**
{% endif %}

{% if member.email %}
Email: [{{ member.email }}](mailto:{{ member.email }})
{% endif %}

{% if member.website %}
[Personal website]({{ member.website }})
{% endif %}

{% if member.twitter %}
Twitter: [@{{ member.twitter }}](https://twitter.com/{{ member.twitter }})
{% endif %}

{% if member.gscholar %}
[Google Scholar]({{ member.gscholar }})
{% endif %}

{{ member.fullbio }}

{% endif %}
{% endif %}
{% endfor %}




<!-- Former members


{% for author in site.data.authors %}
{% assign member = author[1] %}
{% if member.member %}
{% unless member.current %} -->

<!-- ### {{ member.name }}

{% if member.bio %}
**{{ member.bio }}** {% if member.start %}({{ member.start}}{% if member.end %}&ndash;{{ member.end }}{% endif %}){% endif %}
{% endif %}
{% if member.next %}
Next: {{ member.next }}
{% endif %}
{% endunless %}
{% endif %}
{% endfor %} -->
=======
permalink: /Gallery/
layout: single
---

{% for ev in site.data.events %}
  {% include event_gallery.html event=ev %}
  <hr />
{% endfor %}

<style>
.event-image {
  flex: 0 0 auto;   /* keep existing width */
}

.event-image img {
  height: 320px !important;   /* fixed height */
  width: auto !important;     /* keep original width */
  max-width: 100%;            /* safety */
  object-fit: cover !important;
  border-radius: 10px;
  display: block;
}
</style>

