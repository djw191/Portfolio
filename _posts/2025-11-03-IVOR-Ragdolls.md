---
title: "IVOR - Ragdolls and Overkill"
categories:
  - Blog
tags:
  - C#
  - Unity
  - Game
  - IVOR
  - MoonMuse
  - Physics
---
<img src="{{ site.baseurl }}/assets/images/IVOR.png" alt="IVOR logo"><br><br>
Steam link:  <a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">https://store.steampowered.com/app/3033980/IVOR/</a>
<br><br>From August to November 2025 I reworked how enemies die in IVOR.  A big enough hit still gibs them, but anything less now drops them as a ragdoll.
<br><br>Getting the force from the killing blow to carry into the ragdoll took a few attempts.  The solution was a second set of colliders just for the ragdoll, separate from the hitboxes used during combat, and now enemies get knocked back exactly how you'd expect.  I also stopped ragdolls from bumping into the player and handled saving, so a body on the floor doesn't cause problems when a save is loaded.
<br><br>I also added overkill, so if you keep hitting a ragdoll it'll still gib.  After that I did a sound pass, adding and reworking sounds for enemies and weapons.
