---
title: "IVOR - Cleaning Up the Architecture"
categories:
  - Blog
tags:
  - IVOR
  - MoonMuse
  - Game Development
---
<img src="{{ site.baseurl }}/assets/images/IVOR-16x9.png" alt="IVOR logo" style="width: 100%; height: auto;"><br><br>
<a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">Steam Page</a>
<br><br>After showing IVOR at Midwest Gaming Classic 2025, it felt like a good time to clean up and refactor after the crunch to get the game ready to demo.  I spent a lot of that time making the code easier to work in.  I cleared out scripts that were no longer used, organized the rest into namespaces, and removed the last of the singletons, a pattern we were aiming to avoid on this project going forward, which reduced dependencies between systems.
<br><br>Systems like impacts and blood effects now talk through event channels built on ScriptableObjects, so the code is event-driven, nothing needs a hard reference to anything else, and those systems are easier to change.
<br><br>I built tools for the rest of the team too.  All of the game's level info now lives in one place, with a custom inspector that makes it easy to edit, and settings like each level's kill height moved out of scene objects and into that data.
<br><br>On the player side, I added framerate and resolution options and a setting that scales camera shake and weapon kick for players who are sensitive to motion.  I also turned debug tools like god mode into proper settings.
