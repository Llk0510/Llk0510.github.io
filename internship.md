---
layout: page
title: Internship
permalink: /internship/
---

<style>
  .internship-card {
    margin: 1.5rem;
    height: 100%;
  }

  .internship-card .card {
    height: 100%;
    display: flex;
    flex-direction: column;
  }

  .internship-card .card-content {
    flex-grow: 1;
  }

  .internship-description {
    text-align: left;
  }

  .internship-image {
    width: 100%;
    height: 160px;
    object-fit: cover;
  }
</style>

<div class="columns is-multiline is-variable is-4">
  {% for item in site.data.internships %}
    <div class="column is-one-quarter-desktop is-half-tablet is-full-mobile internship-card">
      <div class="card">
        <figure class="image">
          <img class="internship-image" src="{{ item.image }}" alt="{{ item.company }}">
        </figure>
        <div class="card-content">
          <p class="subtitle is-6 has-text-grey has-text-centered">{{ item.company }}</p>
          <p class="subtitle is-7 has-text-grey-light has-text-centered">{{ item.period }}</p>
          <h2 class="title is-5 has-text-centered">{{ item.title }}</h2>
          <p class="internship-description">{{ item.description }}</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>
