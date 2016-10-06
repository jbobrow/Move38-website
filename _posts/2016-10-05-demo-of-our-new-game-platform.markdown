---
title: The first demo of our new game platform
date: 2016-10-05 11:06:00 -04:00
tags:
- fracture
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/oFpwVv5tmO4" frameborder="0" allowfullscreen></iframe>

The video above shows 3 people people playing a prototype of our company's flagship project, a game platform called Automatiles (they may have a different name by the time they ship. Thinky Blinky Bits?)

The game in the video is called Fracture. At the start, the tiles are arranged into bunches so the tiles of one color are clustered together. Then:

1. The players take turns.

2. On your turn, you break the array of tiles into two chunks and put it back together in another formation.

3. When a tile has at least two neighbors but none match its color, it blinks with happiness.

4. The first player whose tiles are all happy at once wins.

Fracture illustrates a some nice things about the system:

1. It's hard to play a game like this with inanimate pieces because players have to manually scan the array to check for happy tiles, which is annoying and game-delaying. Automatiles show you when they're happy and that lets the game shine through.

2. Because the tiles attach and self-align through magnets, the array has a pleasing organization and is easy to manipulate; you can do so not just on the level of single tiles but of whole groups.

3. There's something mesmerizing about them (in our ever so slightly biased opinion)

As this is a prototype there are one or two glitchy moments, but you get the idea. Note fracture won't be playable with the base set, which won't have enough tiles for it. This is just to give you a feel for the system. 

Luckily, there are lots of things the tiles can do because they have brains:  

![automatile-naked.jpg](/uploads/automatile-naked.jpg)

More about that in future posts. In the meantime, here are some ideas we're toying with for initial games: 

1. Solo puzzles where the tiles are happy when they are arranged in some particular configuration, and they get happier the closer you get to it.

2. A flicking game where you're trying to flick the tiles into happy arrangements 

3. Each tile is a magic rune, and each contains its own spell (i.e. exerts unique effects on other tiles). Players take turns casting spells by attaching their runes to a growing array on the table, until some winning condition is reached. Sort of like Magic: The Gathering. Because the system is open source (Arduino!), players could even invent, program, and distribute their own runes, and there could be a metagame economy where players can make fake or real money by selling the runes they invent to other players. 