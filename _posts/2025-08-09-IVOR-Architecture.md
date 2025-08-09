---
title: "IVOR - Cleaning Up the Architecture"
categories:
  - Blog
tags:
  - C#
  - Unity
  - Game
  - IVOR
  - MoonMuse
  - Architecture
  - Tools
---
<img src="{{ site.baseurl }}/assets/images/IVOR.png" alt="IVOR logo"><br><br>
Steam link:  <a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">https://store.steampowered.com/app/3033980/IVOR/</a>
<br><br>Through the middle of 2025 I spent a lot of time making IVOR's code easier to work in.  I cleared out scripts that were no longer used, organized the rest into namespaces, and removed the last of the singletons.
<br><br>In their place, systems like impacts and blood effects now talk through event channels built on ScriptableObjects.  Nothing needs a hard reference to anything else, which made those systems easier to change and let us do things that weren't possible before, like having more than one flying enemy arena in a level.
<br><br>I also built tools for the rest of the team.  All of the game's level info now lives in one place, with a custom inspector that makes it easy to edit, and settings like each level's kill height moved out of scene objects and into that data.  On the player side, I added framerate and resolution options and a setting that scales camera shake and weapon kick for players who are sensitive to motion.
