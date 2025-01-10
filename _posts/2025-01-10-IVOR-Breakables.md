---
title: "IVOR - Breakable Props"
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
<br><br>In January 2025 I joined MoonMuse Entertainment LLC as a volunteer programmer on IVOR, a first-person shooter built in Unity.  My first job was making the world satisfying to shoot at.
<br><br>I built a reusable gibbing system that swaps a prop for its broken pieces when it's destroyed.  I started with barrels, giving each variant its own debris (some lose their lid, others keep a top grate), then extended it to pots, benches, tables, and bookshelves, where the books and loose pages come flying out too.  I also added validation so every piece lands on the right physics layer and nothing breaks if an artist removes a piece later.
<br><br>I also gave the explosive barrel an actual explosion.  Over time the same system grew to cover stained glass windows, crates, kegs, and more, along with hit and break sounds for each.
