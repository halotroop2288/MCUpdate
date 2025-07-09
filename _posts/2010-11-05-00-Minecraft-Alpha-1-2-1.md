---
layout: post
title: Minecraft Alpha v1.2.1 (Server 0.2.3)
wiki-url: Java_Edition_Alpha_v1.2.1
---

The server update is not mandatory, but you might want to update just to make sure.

This is a bugfixes only update:

* Signs on the sides of cacti no longer crash the game
* The player won’t get stuck on the top of the world in multiplayer
* Reverted mob spawning back to the old code, it was far to annoying. I have plans on what to do with this.
* Fixed the leaf particle colors
* Reduced CPU usage for monster spawning, but there’s still a lot of work to be done to reduce lag on SMP servers.
* Attempted to fix the portal dupe bug where you could exit through a different (new) one than the one you entered through.

About the portals, it’s possible that two portals can lead to the same portal in the Nether.
This is because the space down there is compressed by a factor of 8,
and I haven’t come up with a good way to fix this yet.<br>
I might just end up doing an explicit one-to-one binding between portal pairs,
but that’s nontrivial as it should survive the portal being temporarily destroyed.
If you TNT a portal then rebuild it, you’d expect it to still lead to the same place, right?

Hmm.

More bug updates are coming next week, mainly related to survival mode multi player.
