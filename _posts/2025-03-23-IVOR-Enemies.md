---
title: "IVOR - Rebuilding the Enemies"
categories:
  - Blog
tags:
  - C#
  - Unity
  - Game
  - IVOR
  - MoonMuse
  - Game AI
  - Tools
---
<img src="{{ site.baseurl }}/assets/images/IVOR.png" alt="IVOR logo"><br><br>
Steam link:  <a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">https://store.steampowered.com/app/3033980/IVOR/</a>
<br><br>From January to March 2025 I worked through IVOR's enemies, bringing each one over to the game's newer systems and building some new ones from scratch.
<br><br>A big part of that was converting enemy behavior from coroutines into explicit states.  That way an enemy can be saved and loaded in the middle of a fight, even halfway through a multi-step attack, and pick up right where it left off.
<br><br>Every enemy had its own challenge.  The flying enemies move around an arena, so I built a node graph for them to travel along, with checks so nodes never connect through walls and the enemies avoid crashing into each other.  For a spellcaster that teleports around the room, I made a custom Unity editor tool that lets level designers place and aim teleport spots right in the scene.  For walking enemies, I synced animation root motion with the navigation mesh to get rid of foot sliding.  I also gave a gunner proper recoil and had to talk a charging troll out of running off ledges.
<br><br>Along the way I made hitboxes consistent across enemies and added lock-on targets for the player's axe, so combat feels the same no matter what you're fighting.
