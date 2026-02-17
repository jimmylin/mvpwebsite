---
layout: page
title: Clinics & Camps
subtitle: Year-round training opportunities
permalink: /clinics/
---

We offer various clinics and camps throughout the year to help players develop their skills. Whether you're just starting out or looking to refine specific techniques, we have a program for you.

## Upcoming Clinics & Camps

<div class="cards">
{% for clinic in site.clinics %}
  <div class="card">
    <h3>{{ clinic.title }}</h3>
    {% if clinic.dates %}
    <p><strong>Dates:</strong> {{ clinic.dates }}</p>
    {% endif %}
    {% if clinic.cost %}
    <p><strong>Cost:</strong> {{ clinic.cost }}</p>
    {% endif %}
    <p>{{ clinic.excerpt | strip_html | truncatewords: 25 }}</p>
    <a href="{{ clinic.url | relative_url }}" class="btn">Learn More</a>
  </div>
{% endfor %}
</div>

## Types of Programs

### Skills Clinics
Focus on specific skills like serving, passing, setting, or hitting. These clinics are perfect for players who want to improve in particular areas.

### Position Clinics
Specialized training for setters, liberos, middles, and outside hitters. Learn the nuances of your position from experienced coaches.

### Summer Camps
Week-long intensive camps that provide comprehensive training and competitive play. Great for both beginners and advanced players.

### Off-Season Training
Stay sharp during the off-season with our training programs that focus on strength, conditioning, and skill maintenance.

## Why Attend Our Clinics?

- **Expert Instruction**: Learn from experienced coaches with proven track records
- **Small Groups**: Low coach-to-player ratios ensure individual attention
- **Age-Appropriate**: Programs designed specifically for different age groups
- **Flexible Options**: Various times and formats to fit your schedule
- **Affordable**: Competitive pricing with early bird discounts available

## Registration

Registration typically opens 4-6 weeks before each clinic or camp. Space is limited, so early registration is encouraged. Check individual clinic pages for specific registration information and deadlines.

For questions about our clinics and camps, please contact us at {{ site.club_email }} or call {{ site.club_phone }}.
