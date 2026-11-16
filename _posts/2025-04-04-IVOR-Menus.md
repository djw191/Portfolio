---
title: "IVOR - Rebinding and Menus"
categories:
  - Blog
tags:
  - IVOR
  - MoonMuse
  - Game Development
---
<video src="{{ site.baseurl }}/assets/videos/ivor-menus.mp4" poster="{{ site.baseurl }}/assets/images/ivor-menus.jpg" autoplay muted playsinline controls aria-label="Moving through IVOR's main menu, map select, high scores and settings as the camera swings between angles of the 3D scene behind it" style="width: 100%; height: auto;"></video><br><br>
<a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">Steam Page</a>
<br><br>For this period I worked on menus, starting with control rebinding, built on Unity's Input System.  Players can remap both keyboard and controller inputs on the fly.  Conflicting bindings are highlighted until they're fixed, and a rebind can be cancelled partway through.  Those two were not as trivial as I thought they'd be.  Controller settings get their own menu that only shows up when a controller is connected, and it backs out on its own if the controller is unplugged.
<br><br>From there I built out the main menu.  It has a 3D scene behind it, and the camera swings between angles as you move through settings.
