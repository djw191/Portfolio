---
title: "IVOR - Rebinding and Menus"
categories:
  - Blog
tags:
  - C#
  - Unity
  - Game
  - IVOR
  - MoonMuse
  - UI
  - Accessibility
---
<img src="{{ site.baseurl }}/assets/images/IVOR.png" alt="IVOR logo"><br><br>
Steam link:  <a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">https://store.steampowered.com/app/3033980/IVOR/</a>
<br><br>In spring 2025 I took on IVOR's menus, starting with control rebinding.  Players can remap both keyboard and controller inputs on the fly.  Conflicting bindings are highlighted until they're fixed, and a rebind can be cancelled partway through.  Controller settings get their own menu that only shows up when a controller is connected, and it backs out on its own if the controller is unplugged.
<br><br>From there I built out the main menu with a 3D scene behind it and the camera swinging between angles as you move through settings, along with fixes for controller navigation.  I also added a developer console for testing, and later turned debug tools like god mode into proper settings.
<br><br>In 2026 I came back to the rebinding menu to show the actual controller button icons instead of text, which makes it much easier to read at a glance.
