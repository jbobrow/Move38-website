---
title: A board game that can think for itself
date: 2016-10-05 11:06:00 -04:00
tags:
- fracture
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/oFpwVv5tmO4" frameborder="0" allowfullscreen></iframe>

The video above shows 3 people playing a prototype of our flagship project, a game platform called Automatiles (for now; they may have a different name when they ship. Thinky Blinky Bits?)

The pieces are tiny computers. They can think, remember, communicate, and you can load new games into them. They're open source so you can invent your own games for them, and they're very easy to program ([Arduino!](https://www.arduino.cc/)), so they're also a tool for kids to learn code. 

The game in the video is an early demo game called Fracture. At the start, the tiles are arranged so the tiles of each color are clustered together. Then:

1. The players take turns.

2. On your turn, you break the array of tiles into two chunks and put them back together in another formation.

3. When a tile has at least two neighbors but none match its color, it blinks with happiness.

4. The first player whose tiles are all happy at once wins.

Fracture illustrates a few features of the system:

1. It would be hard to play Fracture with inanimate pieces because players would have to manually scan the array to check for happy tiles, which is so annoying it's game-breaking. Automatiles show you when they're happy. They can do all sorts of bookkeeping that would otherwise make all sorts of table games impossible. 

2. Because the tiles attach and self-align via magnets, the array has a pleasing organization, is easy to manipulate, and hard to knock out of place.

3. The tiles were born of our love for the tactile, social nature of board games, and we designed them to retain that magic. When you play, you don’t feel like you’re playing a video game on a table; you feel like you’re playing a board game that can think.

There are one or two glitchy moments in the video because this is a prototype , but you get the idea.

Note Fracture won't be playable with the base set, which won't have enough tiles for it. Luckily, there are lots of things the tiles can do because of their braaaains:

![automatile-naked.jpg](/uploads/automatile-naked.jpg)

So now we get to design a bunch of games, which is my far and away my favorite thing to do in life (we may also hold a design contest if there's interest) Here are a few ideas we're toying with for initial games:

1. **A "hidden movement game"** (think [Scotland Yard](https://en.wikipedia.org/wiki/Scotland_Yard_(board_game))), except there's an AI agent hiding in the tiles and the players have to cooperate to find it. 

2. **Solo puzzles** where the tiles are happy when they are arranged in some particular configuration, and they get happier the closer you get to it.

3. **A flicking game** where you're trying to flick the tiles in order to trigger a chain reaction in the array, or some other kind of neat effect.

4. **A game that teaches you about color-mixing**. You place tiles of different colors together, and they mix to form the color that you'd get when say, mixing paint. Perhaps your goal is to create some particular color palette before your opponents create theirs.

5. **Each tile is a magic rune**, and each contains its own spell (exerts a unique effects on other tiles). Players take turns casting spells by attaching their runes to a growing array on the table, until some winning condition is reached. Because the system is open source, players could invent, program, and distribute their own runes. There could even be a metagame economy where players make fake or real money by selling the runes they invent to other players.

While we're at it, here's a poll where you can tell us which of the above sounds most interesting to you.

There's a lot more where that came from. Here's our current stack of game concepts for the system:

![tile-concepts.JPG](/uploads/tile-concepts.JPG)

That's right, we design with notecards in a wood-paneled room. We don't live in the future ALL the time.

<!-- Begin MailChimp Signup Form -->
<link href="//cdn-images.mailchimp.com/embedcode/classic-10_7.css" rel="stylesheet" type="text/css">
<style type="text/css">
\#mc_embed_signup{background:#fff; padding:0 10px 0 0px; margin:0 0 20px 0; max-width:300px; clear:left;}
</style>
<div id="mc_embed_signup">
<form action="//automatiles.us14.list-manage.com/subscribe/post?u=7857fa104de3ffc5bbe78d94c&id=c82a234f7c" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
<div id="mc_embed_signup_scroll">
<div class="mc-field-group">
<label for="mce-EMAIL">Email Address</label>
<input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL">
</div>
<div id="mce-responses" class="clear">
<div class="response" id="mce-error-response" style="display:none"></div>
<div class="response" id="mce-success-response" style="display:none"></div>
</div>    <!-- real people should not fill this in and expect good things - do not remove this or risk form bot signups-->
<div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_7857fa104de3ffc5bbe78d94c_c82a234f7c" tabindex="-1" value=""></div>
<div class="clear"><input type="submit" value="Subscribe" name="subscribe" id="mc-embedded-subscribe" class="button"></div>
</div>
</form>
</div>
<script type='text/javascript' src='//s3.amazonaws.com/downloads.mailchimp.com/js/mc-validate.js'></script><script type='text/javascript'>(function($) {window.fnames = new Array(); window.ftypes = new Array();fnames\[0\]='EMAIL';ftypes\[0\]='email';fnames\[1\]='FNAME';ftypes\[1\]='text';fnames\[2\]='LNAME';ftypes\[2\]='text';}(jQuery));var $mcj = jQuery.noConflict(true);</script>
<!--End mc_embed_signup-->

-[Nick Bentley](https://nickbentleygames.wordpress.com/)