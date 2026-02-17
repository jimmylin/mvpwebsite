---
layout: page
title: Our Teams
subtitle: Meet our competitive volleyball teams
permalink: /teams/
---

## 2024-2025 Season Teams

We offer teams for various age groups and skill levels. Each team is carefully constructed to provide competitive opportunities while fostering player development.

<div class="cards">
{% for team in site.teams %}
  <div class="card team-card">
    <h3>{{ team.title }}</h3>
    {% if team.age_group %}
    <p><strong>Age Group:</strong> {{ team.age_group }}</p>
    {% endif %}
    {% if team.coach %}
    <p><strong>Coach:</strong> {{ team.coach }}</p>
    {% endif %}
    <p>{{ team.excerpt | strip_html | truncatewords: 20 }}</p>
    <a href="{{ team.url | relative_url }}" class="btn">Learn More</a>
  </div>
{% endfor %}
</div>

## Tryout Information

Tryouts for the upcoming season are typically held in [Month]. All interested players are encouraged to attend, regardless of experience level. We evaluate players based on:

- Technical skills (passing, setting, hitting, serving, blocking)
- Volleyball IQ and court awareness
- Attitude, coachability, and work ethic
- Athleticism and physical tools

Stay tuned for specific tryout dates and registration information!

## Team Fees & Commitment

Playing club volleyball is a significant commitment. Team fees typically include:

- Professional coaching and training
- Tournament entry fees
- Team uniforms and gear
- Court time and facility costs
- Administrative expenses

We offer payment plans and limited scholarships based on financial need. Contact us to learn more.
