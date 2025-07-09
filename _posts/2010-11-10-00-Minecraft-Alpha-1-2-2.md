---
layout: post
title: Minecraft Alpha v1.2.2 (Server 0.2.4)
wiki-url: Java_Edition_Alpha_v1.2.2
---

A whole pile of bug fixes in this one. There’s still a lot more to do, coming over the next couple of weeks or so.

General fixes:
* players and mobs in lava or fire no longer spam sound effects
* getting hit with a higher damage while recovering from a smaller one now works as intended
* lava flows further in the Nether
* zombie pigs eventually forgives
* added support for custom skin packs
* fixed duplicate buttons when resizing screens
* zombie pigs and ghasts no longer get hurt by fire or lava
* fixed volume sliders now saving properly

Multiplayer fixes:
* hellworld=true no longer overwrites old save chunks. Player positions will still break if you switch it on a running server, though
* boats are now visible to other players
* minecarts move nicer
* fishing kinda sorta works, but needs more work
* sheep and cows look like sheep and cows now
* buckets work now
* fixed stairs being really difficult to destroy
* increased the timeout before “Took too long to log in”
* made it possible to ride carts and boats
* added (after lots of work) the ability to steer server-side boats
* added “no-animals” setting. if true, animals will immediately vanish
* added support for more animation settings. Currently it’s just the “riding” animation, but the same system will be used for sneaking

To make a texture pack, make a zip file that contains the files you wish to replace,
then place that zip file in the texture pack folder.
There’s a handy button ingame to open that folder immediately.

If you place a “pack.png” file in the root of the zip file, it’ll show up as a preview icon.
Please make sure it’s square, and of an even 2^x size. For example, 128x128 pixels.<br>
If you place a “pack.txt” file in the root of the zip file,
the first two lines will show up as a description for the texture pack.
