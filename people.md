---
layout: page
title: People
---

## Principal Investigator

<div class="people-center">
{% for person in site.data.people.faculty %}
  <div class="person-card">
    <img src="{{ person.img }}" alt="{{ person.name }}">
    <h3>{{ person.name }}</h3>
    <p>{{ person.role }}</p>

    <div class="person-links">
      {% if person.google_scholar %}
        <a href="{{ person.google_scholar }}" target="_blank">
          <i class="ai ai-google-scholar"></i>
        </a>
      {% endif %}

      {% if person.linkedin %}
        <a href="{{ person.linkedin }}" target="_blank">
          <i class="fab fa-linkedin"></i>
        </a>
      {% endif %}

      {% if person.bluesky %}
        <a href="{{ person.bluesky }}" target="_blank">
          <i class="fa-solid fa-cloud"></i>
        </a>
      {% endif %}
    </div>

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