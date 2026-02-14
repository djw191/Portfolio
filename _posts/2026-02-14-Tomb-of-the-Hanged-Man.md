---
title: "Global Game Jam 2026 - Tomb of the Hanged Man"
categories:
  - Blog
tags:
  - MoonMuse
  - Game Development
  - Game Jam
---
<img src="{{ site.baseurl }}/assets/images/TombOfTheHangedMan.png" alt="Tomb of the Hanged Man banner"><br><br>
<a href="https://moonmusegames.itch.io/tomb-of-the-hanged-man" target="_blank">itch.io Page</a>
<br><br>MoonMuse participated in Global Game Jam 2026 again, as is now tradition.  The theme was Mask, and we took on the diversifier "Many hands make light work", which asks for a game meant to be played with four or more players.
<br><br>Tomb of the Hanged Man is an online co-op horror game made in Unity.  You enter the tomb alone or with friends and have to find four masks hidden in the catacombs to escape, while avoiding ancient traps and the spirit that lurks there.
<br><br>I was one of two programmers on a team of six.  Networking was left to me.  I set up hosting and joining with Unity's Netcode for GameObjects and Relay, so friends can join with a code, and added a direct connection option alongside it.  I also got proximity voice chat working with Vivox, so you only hear the players near you.
<br><br>Then I built the traps: spikes, trapdoors, darts, and gas vents.  I also wired up the flow of a round, from the start door through to respawns and the win condition.
<br><br>After the jam we kept going for a couple of weeks and put out a 1.1 update.  For that I added spectating once you die, a pause menu, player nameplates, timers on the masks, torches that can be lit and put out, and a rolling boulder trap.
