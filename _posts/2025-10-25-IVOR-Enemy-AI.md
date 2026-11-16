---
title: "IVOR - Smarter Enemies"
categories:
  - Blog
tags:
  - IVOR
  - MoonMuse
  - Game Development
---
<video src="{{ site.baseurl }}/assets/videos/ivor-enemy-ai.mp4" poster="{{ site.baseurl }}/assets/images/ivor-enemy-ai.jpg" autoplay muted playsinline controls aria-label="The custom patrol editor in Unity's Scene view, drawing an enemy's patrol route between its points" style="width: 100%; height: auto;"></video><br><br>
<a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">Steam Page</a>
<br><br>I gave IVOR's enemies a sense of awareness.  Every enemy now shares a base AI alongside its own controller, a finite state machine that moves between patrolling, alert, and aggressive states.
<br><br>Enemies notice you with a detection radius for things right next to them, plus a vision cone with line-of-sight checks for everything else, so walls and corners actually matter.  Getting shot or caught in an explosion sets them off immediately, straight to aggressive.
<br><br>I also built a patrol system with pauses at each point, separate patrol and chase speeds, and a custom editor that draws the patrol route in the scene so level designers can see exactly where an enemy will walk.
<br><br>This is now rolled out to every enemy that walks the NavMesh, and I've been tuning and fixing edge cases with the level designers since.
