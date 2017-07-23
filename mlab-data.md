---
layout: default
title: Working with data
permalink: /mlab-data/
---

**Here is a very annoying thing to know!!** If you open this data in excel and save it, it will stop working as a csv. Use google sheets instead. Or, even better, work with data that is yaml or json.

{% for novel in site.data.end-19c-epi %}
  <p>
    The book "<em>{{ novel.title }}""</em> was written by {{ novel.author }}. Then, it said, "{{ novel.a }}"
  </p>
{% endfor %}


{% for monument in site.data.mlab2 %}
  <div>
    <h3><strong>{{ monument.name }}</strong></h3>
    <img src="{{ monument.form_image_b }}" />
    <hr />
  </div>
{% endfor %}
