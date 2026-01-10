---
title: "Leadership"
permalink: /leadership/
layout: single
---


{% for ev in site.data.leadership %}
  {% include event_leadership.html event=ev %}
  <hr />
{% endfor %}

<style>
.event-image {
  flex: 0 0 auto;   /* keep existing width */
}

.event-image img {
  height: 150px !important;   /* fixed height */
  width: auto !important;     /* keep original width */
  max-width: 100%;            /* safety */
  object-fit: cover !important;
  border-radius: 10px;
  display: block;
}
</style>
