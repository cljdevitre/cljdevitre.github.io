---
layout: page
title: People
---

## Principal Investigator

<div class="people-center">
{% for person in site.data.people["Principal Investigator"] %}
  <div class="person-card">
    <img src="{{ person.img }}" alt="{{ person.name }}">
    <h3>{{ person.name }}</h3>
    <p>{{ person.role }}</p>

  <div class="person-links">

    {% if person.google_scholar %}
      <a href="{{ person.google_scholar }}" target="_blank" title="Google Scholar">
        <i class="ai ai-google-scholar"></i>
      </a>
    {% endif %}

    {% if person.linkedin %}
      <a href="{{ person.linkedin }}" target="_blank" title="LinkedIn">
        <i class="fab fa-linkedin"></i>
      </a>
    {% endif %}

    {% if person.bluesky %}
      <a href="{{ person.bluesky }}" target="_blank" title="Bluesky">
        <i class="fa-solid fa-cloud"></i>
      </a>
    {% endif %}

    {% if person.orcid %}
      <a href="{{ person.orcid }}" target="_blank" title="ORCID">
        <i class="ai ai-orcid"></i>
      </a>
    {% endif %}

  </div>


  </div>
{% endfor %}
</div>


## Graduate Students

<div class="people-grid">
{% for person in site.data.people["Graduate students"] %}
  <div class="person-card">
    {% if person.img %}
      <img src="{{ person.img }}" alt="{{ person.name }}">
    {% endif %}
    <h3>{{ person.name }}</h3>
    <p>{{ person.role }}</p>
  </div>
{% endfor %}
</div>


## Undergraduate Students

<div class="people-grid">
{% for person in site.data.people["Undergraduate students"] %}
  <div class="person-card">
    {% if person.img %}
      <img src="{{ person.img }}" alt="{{ person.name }}">
    {% endif %}
    <h3>{{ person.name }}</h3>
    <p>{{ person.role }}</p>
  </div>
{% endfor %}
</div>
