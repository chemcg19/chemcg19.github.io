---
title: "About Me"
layout: default
permalink: /about-me/
---

### About Me

Information about my professional experience and goals.

skills:
  - name: "Unity"
    icon: "fab fa-fw fa-unity"
    badges: ["C#", "Game Dev"]
    text: "Built multiple prototypes and a published jam game."
    years: 2
  - name: "Game Design"
    icon: "fas fa-fw fa-gamepad"
    badges: ["Game Mechanics", "Levels", "UI"]
    text: "Designed mechanics, levels, and player feedback loops."
    level_label: "Beginner

{% assign skills = include.skills | default: page.skills %}

{% if skills %}
<div class="skills {{ include.class }}">
  {% for skill in skills %}
    <div class="skill-card">
      {% if skill.icon %}
        <div class="skill-card__icon"><i class="{{ skill.icon }}" aria-hidden="true"></i></div>
      {% endif %}
      <div class="skill-card__body">
        <h3 class="skill-card__title">{{ skill.name }}</h3>
        {% if skill.badges %}
          <ul class="skill-card__badges">
            {% for badge in skill.badges %}
              <li>{{ badge }}</li>
            {% endfor %}
          </ul>
        {% endif %}
        {% if skill.text %}
          <p class="skill-card__text">{{ skill.text | markdownify | remove: "<p>" | remove: "</p>" }}</p>
        {% endif %}
        {% if skill.years %}
          <div class="skill-card__meta">
            <span class="skill-card__meta-label">Experience</span>
            <span class="skill-card__meta-value">{{ skill.years }} years</span>
          </div>
        {% elsif skill.level_label %}
          <div class="skill-card__meta">
            <span class="skill-card__meta-label">Level</span>
            <span class="skill-card__meta-value">{{ skill.level_label }}</span>
          </div>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>
{% endif %}
