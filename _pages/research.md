---
layout: archive
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

# <span style="color:#77AFC7">Work in progress</span>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'workinprogress' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<span style="color:white">Publications</span>

# <span style="color:#77AFC7">Working papers</span>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'workingpaper' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<span style="color:white">Publications</span>


# <span style="color:#77AFC7">Publications</span>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'publication' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

<span style="color:white">Publications</span>


# <span style="color:#77AFC7">External reports</span>
{% for post in site.publications reversed %}
  {% if post.pubtype == 'external' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}

