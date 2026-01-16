---
title: "IVOR - Performance and Lighting"
categories:
  - Blog
tags:
  - C#
  - Unity
  - Game
  - IVOR
  - MoonMuse
  - Optimization
  - Lighting
---
<img src="{{ site.baseurl }}/assets/images/IVOR.png" alt="IVOR logo"><br><br>
Steam link:  <a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">https://store.steampowered.com/app/3033980/IVOR/</a>
<br><br>At the end of 2025 I shifted to performance and lighting as IVOR moved to Unity's Universal Render Pipeline.  I started with the biggest wins: mesh LODs so distant objects use simpler models, and GPU occlusion culling so the game skips drawing things the player can't see.
<br><br>Then I went through the levels one at a time.  I set up baked lighting and adjusted model import settings so lightmaps came out clean, then added volumetric lighting, a physically based sky, screen space global illumination, reflection probes, and post-processing for each level.  A lot of that was just playing with brightness values until the mood felt right.
<br><br>I also optimized the fire effects.  Fire now spreads by casting rays in an evenly distributed sphere to find where flames should land, and the effects themselves are cheaper to run.
