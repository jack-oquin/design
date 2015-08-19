---
layout: default
title: ROS2 Design
html_title: Design
---

# ROS 2.0 Design

This site is repository of articles which are designed to inform and guide the ROS 2.0 design efforts.
The goal of the ROS 2.0 project is to leverage what is great about ROS 1.x and improve what isn't.

If you would like to contribute, checkout the [contribute]({{ site.baseurl }}/contribute.html) page to learn how.

The best mailing list for discussing these topics is [ros-sig-ng-ros@googlegroups.com](mailto:ros-sig-ng-ros@googlegroups.com).
 You can view the archives [here](https://groups.google.com/forum/?fromgroups#!forum/ros-sig-ng-ros)

# Articles

Here is a list of the articles (white papers) which have been written so far. These articles should serve as an excellent entry point for anyone wanting to join the conversation about any of the ROS 2.0 topics.

{% assign sorted_pages = site.pages | sort:"name" %}
{% for p in sorted_pages %}
    {% if p.url contains 'articles/' and p.published == true %}
----

#### [{{ p.title }}]({{ site.baseurl }}{{ p.url }})

> {{ p.abstract }}
    {% endif %}
{% endfor %}

----

<div class="unpublished" style="display: none;" markdown="1">
# Unpublished Articles

These articles are not finished or maybe not even started yet:

{% assign sorted_pages = site.pages | sort:"name" %}
{% for p in sorted_pages %}
    {% if p.url contains 'articles/' and p.published != true %}
----

#### [{{ p.title }}]({{ site.baseurl }}{{ p.url }})

> {{ p.abstract }}
    {% endif %}
{% endfor %}

----
</div>
