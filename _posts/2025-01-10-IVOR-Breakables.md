---
title: "IVOR - Breakable Props"
categories:
  - Blog
tags:
  - IVOR
  - MoonMuse
  - Game Development
---
<video src="{{ site.baseurl }}/assets/videos/ivor-breakables.mp4" poster="{{ site.baseurl }}/assets/images/ivor-breakables.jpg" autoplay muted playsinline controls aria-label="Props breaking into pieces in IVOR when shot, including an exploding barrel" style="width: 100%; height: auto;"></video><br><br>
<a href="https://store.steampowered.com/app/3033980/IVOR/" target="_blank">Steam Page</a>
<br><br>I recently joined MoonMuse Entertainment LLC as a contract programmer.  Their main project at the moment is IVOR, a retro first-person shooter built in Unity, and I was brought on to work on it through to release.
<br><br>My first task after joining was to make the world satisfying to shoot at.  Specifically, I built a reusable gibbing system that swaps a prop for its broken pieces when it's destroyed.  I started with barrels, giving each variant its own debris (some lose their lid, others keep a top grate), then extended it to pots, benches, tables, and bookshelves, where the books and loose pages come flying out when they're destroyed.  I also added validation so every piece lands on the right physics layer, where the player can push the pieces around without them affecting player movement, and nothing breaks if an artist removes a piece later.
<br><br>I also implemented a new barrel type, the exploding barrel, which reuses the cannon's VFX for its explosion.
