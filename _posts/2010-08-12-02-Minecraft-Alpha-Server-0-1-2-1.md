---
layout: post
title: Minecraft Alpha Server 0.1.2_01
wiki-url: Java_Edition_Alpha_server_0.1.2_01
---

TkTech contacted me over IRC and pointed out a flaw in the authentication scheme
that would let hackers connect to server a player was last logged into.

This has been solved now by turning the login key into a proper nonce
that gets changed every time a new TCP connection is made to the server.

If you worry about name impersonation, I suggest you get this update ASAP.
