---
title: "IVOR - Rebuilding the Enemies"
categories:
  - Blog
tags:
  - IVOR
  - MoonMuse
  - Game Development
---
<video src="{{ site.baseurl }}/assets/videos/ivor-enemies.mp4?v=2" poster="{{ site.baseurl }}/assets/images/ivor-enemies.jpg?v=2" autoplay muted playsinline controls aria-label="The melee troll running at the player and launching off a ledge in IVOR" style="width: 100%; height: auto;"></video><br><br>
<a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">Steam Page</a>
<br><br>I transitioned to working on enemies.  Many existing monsters needed changes and revisions to bring them in line with how the game had evolved.  As well, I began to work on implementing all-new enemies, like the melee troll variant.
<br><br>A big part of that was converting enemy behavior into explicit state machines.  That way an enemy can be saved and loaded in the middle of a fight, even halfway through a multi-step attack, and pick up right where it left off.  This is important since we use an in-house system that saves the entire state of the game at any moment.
<br><br>Every enemy had its own challenge.  The flying enemies travel along a node graph around their arena, and those nodes used to be placed by hand.  I built a tool that lets designers select a region and generates an irregularly spaced 3D node graph for it, automatically working around static obstacles.  For a ranged enemy that teleports around the room, I made a custom Unity editor tool that lets level designers place and aim teleport spots right in the scene.  For walking enemies, I synced animation root motion with the NavMesh to get rid of foot sliding.  The cannon troll got proper recoil.
<br><br>The melee troll was the hardest to get working.  For it to fly off a ledge in a satisfying way I had to work around Unity's navigation mesh system, and then I had to talk it out of charging off ledges for no reason.
<br><br>Finally, I made hitboxes consistent across enemies, so combat feels consistent and fair no matter what you're fighting.
