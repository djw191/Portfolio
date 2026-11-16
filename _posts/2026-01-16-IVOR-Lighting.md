---
title: "IVOR - Performance and Lighting"
categories:
  - Blog
tags:
  - IVOR
  - MoonMuse
  - Game Development
---
{% include compare.html before="/assets/images/ivor/hdrp-arena.jpg?v=3" after="/assets/images/ivor/urp-arena.jpg?v=3" before_label="HDRP" after_label="URP" alt="The start of round 1 in one of IVOR's arenas" caption="Drag to compare the last HDRP build (left) with the current URP build (right). Screenshots matched for overall brightness and saturation." %}
<a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">Steam Page</a>
<br><br>My next task was to dig into performance, using the Unity Profiler to find anywhere we could optimize.  Some low-hanging fruit were mesh LODs so distant objects use simpler models, and GPU occlusion culling so the game skips drawing things the player can't see without taxing the CPU, which is our main constraint at the moment.  Then we moved IVOR to Unity's Universal Render Pipeline (URP), which seemed like the best way to claw back CPU time, since HDRP's CPU cost was very taxing for us.  I used Claude Code to help build a temporary tool that converted our materials between pipelines, which got us moved over with far fewer hours of manual work, though the whole team still had to do some tweaks and checks.
<br><br>After the move I went through the levels one at a time.  I tried Unity's built-in lightmapping first, and for us it didn't work very well, so much so that we dropped the idea altogether.  The bake times were too long for prototyping and the file sizes were too large.  From there I added back volumetric lighting, which we had lost in the transition but was vital to the identity of our game.  Tweaking the look afterwards was very finicky, mostly messing with effects until we got back to how we wanted the game to look, just much more performant.
