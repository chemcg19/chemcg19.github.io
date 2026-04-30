---
title: "About Me"
layout: default
permalink: /about-me/
skills:
  - name: "Unity"
    icon: "fab fa-fw fa-unity"
    badges: ["C#", "Game Dev"]
    text: "Built multiple demos both independantly and in a team."
    years: 4
  - name: "Game Design"
    icon: "fas fa-fw fa-gamepad"
    badges: ["Game Mechanics", "Levels", "UI", "Audio and Lighting"]
    text: "Designed mechanics, levels, prototyped levels and features, and implemented features like lighting and UI elements, etc."
    level_label: "Intermediate/Proficient"
    years: 4
  - name: "C#"
    icon: "fas fa-fw fa-gamepad"
    text: "Coded multiple intricate mechanics on a wide variety of game objects, including player, enemy, NPC, follower, and environment/interactable scripts."
    level_label: "Intermediate"
    years: 3
  - name: "Modelling and Texturing"
    icon: "fas fa-fw fa-gamepad"
    text: "Built multiple 3D models in Maya and textured them myself using Substance Painter and Photoshop, imported them into Unity with proper scaling and texture maps. Created multiple of my own 2D sprites for my games."
    level_label: "Beginner"
    years: 4
---

# About Me

<div style="display:flex; flex-wrap:wrap; gap:2rem; align-items:flex-start;">
<!-- LEFT: text content -->
<div style="flex:1 1 250px; min-width:250px;">
<h2>Hi, I'm Che, a games design and development student based in Derry</h2>
<p>
I am currently studying at Ulster University, developing my skills and passion for working on both solo projects and group projects. I am efficient and reliable in Unity and C#, and am also developing my skills in modelling, texturing, and 2D art.
in module CRE135: 2D Game Creation.
</p>
</div>
<!-- RIGHT: video/content area -->
<div style="flex:1 1 250px; min-width:250px;">
<!-- Replace this placeholder with a YouTube iframe or a video tag -->
{% include figure image_path="/assets/images/GameJam2024" alt="Game Jam screenshot" caption="My Game Jam 2024 Submission" %}
</div>
</div>

## My Skills {#skills}
{% include skills skills=page.skills %}
