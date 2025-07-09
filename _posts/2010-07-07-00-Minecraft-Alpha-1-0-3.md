---
layout: post
title: Minecraft Alpha v1.0.3
wiki-url: Java_Edition_Alpha_v1.0.3
---

Getting the levels to support more than one player turned out to be a bigger rewrite than I thought.
There was a surprising amount of `level.getPlayer()` calls,
so I added a `level.getNearestPlayer(x, y, z)`, which worked great as a substitute for most of the calls.
Another issue was the tile polling. In the original version,
tiles between two players would get polled twice as frequently as tiles only near a single player.
This also affected the mob spawner code.
The solution there was to build a set of all unique chunks near players,
which turns out to be handy when I do the memory caching of terrain data anyway.

I haven’t actually implemented any multiplayer support in the client yet, but I did do some work on it,
which leads up to version 1.0.3:

* The pathfinder now works for hills. Except for spiders. Of course.
* Generally more convincing mob idling behavior. They’ll stand still more, looking around at their surroundings
* Monster sounds
* Ambient cave noises

Tomorrow is Thursday, then it’s Seecret Friday time, so it doesn’t seem like I’ll have anything testable this week.
