---
title: When board game components can think, how do you tell them what to do?
date: 2016-10-15 12:56:00 -04:00
---

Last week we offered [a peek](http://move38.com/blog/a-board-game-that-thinks/) at the game platform we're developing. It's called Automatiles (but I'm hesitant to use that name because it might be called something different by the time we sell it). 

![Fracture_hands_01.jpg](/uploads/Fracture_hands_01.jpg)

To recap:

> the game pieces are little computers. They can think, remember, communicate with players and each other, and you can load new games into them. They’re open source so you can invent your own games for them, and they’re easy to program (Arduino!), so they’re also a tool for kids to learn code.

Here's a video we recorded at Indicade over the weekend:

\[insert video\]

Today I'm discussing a design issue we're facing. Maybe you'll read it and give us your opinion. It has to do with this bit: 

> you can load new games into them

The question is: how? 

Right now, you have to load games into each tile separately by removing their covers and getting into the hardware, like this: 

![IMG_0992.JPG](/uploads/IMG_0992.JPG)

...which is ok for tinkerers and programmers but not for people who just want to play games. We've learned 6-12 year olds are especially in love with the tiles, so switching games must be easy for them. 

We need a loading method with the following characteristics:

1. downloading a game should happen at the press of a button

2. a game should download into all the tiles at once, instead of one-by-one. 

3. downloading shouldn't require taking the pieces apart.

Luckily we have two good options, but we haven't decided which to implement: 

## Option #1 - download from phone via Bluetooth

One of the tiles will communicate with your phone by Bluetooth, and there'll be an app that comes with the tiles. When you want to play a new game, you open the app and select the game you want to play. The phone zaps the instructions to the tile with Bluetooth, and when that tile is attached to all the other tiles, it sends instructions to them via their normal communication (infrared)

## Option #2  - games on tiles

Each tile comes with a game preprogrammed on it. When you want to play a new game, you attach the tile with the game you want to all the other tiles and hold and press its top. It then sends instructions to all the other tiles. 

Here are the strengths and weaknesses of these options as we now understand them: 

\[insert table\]

But we're not sure we fully understand the parameters of the problem yet. If you have a preference for one of these options, or think of strengths or weaknesses we've missed, let us know in the comments. That's basically our entire reason for posting this. We want to suck all the knowledge from your delicious brain and leave you a desiccated ignorant husk.  

\[solicit team members\]