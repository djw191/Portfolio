---
title: "Haskell Project - Rewriting the Mythos Server"
categories:
  - Blog
tags:
  - C#
  - Unity
  - Haskell
  - Functional Programming
  - School Project
---
<img src="{{ site.baseurl }}/assets/images/haskell.png"><br><br>
github link:  <a href="https://github.com/Zaidis/MAGD_488/tree/SSL-Haskell" target="_blank">https://github.com/Zaidis/MAGD_488/tree/SSL-Haskell</a><br>
<br><br>In my Spring 2024 semester at UWM I took a special topics course on functional programming.  The first half of the course was getting familiar with the functional style of coding and haskell in specific, and the second half was working on a project that had real applications, not just a proof of concept.
<br><br>Because of the advantages of haskell, I immediately thought of my undergraduate capstone Myhos.  It had a socket server that I wrote in C#, but it was a little rushed and didn't have proper security implemented.  So what I did is rewrite the sever from the ground up so that it had feature parity with the original
server.  The game itself did need updating for compatibility, but not because of the language change, but because of the added security in the properly implemented TLS.  
<br><br>The game works as expected online and the new server has eliminated some bugs that the old one had.  A lot of the issues the old server had to do with multithreading to support multiple connections interacting with each other.  Haskell allows simple ways of achieving multithreading while maintaining data safety and
avoiding common object oriented pitfalls.
