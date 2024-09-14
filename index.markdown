---
layout: home
---

# Welcome to My Portfolio

Here you'll find information about my projects and blog posts.

## Featured Projects

{% for project in site.projects limit:3 %}
  <h3>
    <a href="{{ project.url }}">
      {{ project.title }}
    </a>
  </h3>
  <p>{{ project.description }}</p>
{% endfor %}

[View All Projects](/projects/)

## Latest Blog Posts

{% for post in site.posts limit:3 %}
  <h3>
    <a href="{{ post.url }}">
      {{ post.title }}
    </a>
  </h3>
  <p>{{ post.date | date_to_string }}</p>
{% endfor %}

[View All Posts](/blog/)