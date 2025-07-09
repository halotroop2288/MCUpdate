---
layout: post
title: Minecraft Alpha v1.0.5
wiki-url: Java_Edition_Alpha_v1.0.5
---

+ Added snowballs. You can throw them, but they deal no damage
+ Added craftable snow blocks
* Fixed building on snow bug
* Fixed ice rendering bug
* Signs no longer require a free block above them when placing them
* The game no longer saves the level when it crashes. Saving on crashes sometimes broke save files, and that’s not good.

Work on Multiplayer is going really well, and it’s actually starting to get fun.
I implemented a fancy mapping between players and level chunks today.
It automatically sends terrain data as players move,
and keep track of exactly what players are in range of what chunks, for efficient broadcasting.
I will also use it to buffer block changes within chunks to send them as a single compound command,
saving a whole bunch of bandwidth.

And there’s now a
`replaceRegion(int x, int y, int z, byte xSize, byte ySize, byte zSize, byte[] gzipCompressedData)` command.
The only limitation is that y and ySize both have to be even, but it can be used to quickly send large level updates,
and it’s implemented almost directly into the Level class itself,
so it can be used to load/replace arbitrary regions of the map.
It will probably be quite useful for server mods such as area backups
or for resetting the arena between levels in a Spleef mod.

[edit:]

And now snow shouldn’t fall through glass anymore.
