---
title: "IVOR - Ragdolls and Overkill"
categories:
  - Blog
tags:
  - IVOR
  - MoonMuse
  - Game Development
---
<video src="{{ site.baseurl }}/assets/videos/ivor-ragdolls.mp4" poster="{{ site.baseurl }}/assets/images/ivor-ragdolls.jpg" autoplay muted playsinline controls aria-label="Enemies in IVOR dropping as ragdolls when shot, then gibbing when the player keeps hitting the body" style="width: 100%; height: auto;"></video><br><br>
<a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">Steam Page</a>
<br><br>I reworked how enemies die in IVOR.  A big enough hit still gibs them (breaks their body into chunks that fly around), but anything less now drops them as a ragdoll.
<br><br>Getting the force from the killing blow to carry into the ragdoll took a few attempts.  The solution was a second set of colliders just for the ragdoll, separate from the hitboxes used during combat, and now enemies get knocked back exactly how you'd expect.  Ragdolls also don't directly affect the player's movement.  Instead, they can be pushed by the player or other enemies, and knocked around by weapon hits.
<br><br>Then I added overkill, so if you keep hitting a ragdoll it'll still gib.  After that I did a sound pass, adding and reworking sounds for enemies and weapons.
