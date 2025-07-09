---
layout: post
title: Minecraft Alpha v1.0.7
wiki-url: Java_Edition_Alpha_v1.0.7
---

Today was a very slow day, with me working out some of the kinks in Multiplayer
and starting to work on reducing the network usage.

For the last couple of versions of Minecraft (or longer?),
there’s been a bug where the player would get stuck in a weird stuttering mode sometimes.

While working on the multiplayer fixes,
I ran into some code which looked suspicious (keeping track of the last zone a player was in),
and it turned out to be totally broken in several places,
such as when the player got teleported (entering/exiting a vehicle)
or when loading and the player is right on the edge of a zone.

So I fixed that, and released client version 1.0.7. Let me know how it works in the comments, please. :-D
