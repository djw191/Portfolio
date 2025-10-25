---
title: "IVOR - Smarter Enemies"
categories:
  - Blog
tags:
  - C#
  - Unity
  - Game
  - IVOR
  - MoonMuse
  - Game AI
---
<img src="{{ site.baseurl }}/assets/images/IVOR.png" alt="IVOR logo"><br><br>
Steam link:  <a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">https://store.steampowered.com/app/3033980/IVOR/</a>
<br><br>In fall 2025 I gave IVOR's enemies a sense of awareness.  Every enemy now shares a base AI that moves between idle, patrolling, alert, and aggressive states.
<br><br>Enemies notice you with a detection radius for things right next to them, plus a vision cone with line-of-sight checks for everything else, so walls and corners actually matter.  Getting shot or caught in an explosion alerts them immediately.  I also built a patrol system with pauses at each point, separate patrol and chase speeds, and a custom editor that draws the patrol route in the scene so level designers can see exactly where an enemy will walk.
<br><br>After rolling this out to every enemy that walks the navigation mesh, I spent the following weeks tuning and fixing edge cases with the level designers.  Later on I added touches like ranged enemies firing at where they last saw you and small random speed differences so groups don't move in lockstep.
