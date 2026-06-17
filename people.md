---
layout: page
title: People
---

## Faculty

<div class="people-grid">
{% for person in site.data.people.faculty %}
  <div class="person-card">
    <img src="{{ person.img }}" alt="{{ person.name }}">
    <h3>{{ person.name }}</h3>
    <p>{{ person.role }}</p>
    {% if person.url %}
      <a href="{{ person.url }}">Profile</a>
    {% endif %}
  </div>
{% endfor %}
</div>

## Students

<div class="people-grid">
{% for person in site.data.people.students %}
  <div class="person-card">
    <img src="{{ person.img }}" alt="{{ person.name }}">
    <h3>{{ person.name }}</h3>
    <p>{{ person.role }}</p>
  </div>
{% endfor %}
</div>