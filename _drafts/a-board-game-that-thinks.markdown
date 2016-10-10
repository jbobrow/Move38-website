---
title: A board game that can think for itself
date: 2016-10-05 11:06:00 -04:00
tags:
- fracture
---

<iframe width="594" height="334" src="https://www.youtube.com/embed/oFpwVv5tmO4" frameborder="0" allowfullscreen></iframe>

The video above shows 3 people playing a prototype of our flagship project, a game platform called Automatiles (for now; it may have a different name when it ships. Thinky Blinky Bits?)

The game pieces are little computers. They can think, remember, communicate with players and each other, and you can load new games into them. They're open source so you can invent your own games for them, and they're easy to program ([Arduino!](https://www.arduino.cc/)), so they're also a tool for kids to learn code.

The game in the video is an early demo called Fracture, a game about maximizing diversity. It was designed in collaboration with [Celia Pearce](http://www.northeastern.edu/camd/gamedesign/people/celia-pearce/), director of [Northeastern’s game design program](http://www.northeastern.edu/camd/gamedesign/). Jon told her they could go from concept to implementation in 3 hours. In fact they ended up going from *no* concept to implementation in that time. Here's how it works:

At the start, the tiles are arranged in same-color clusters. Then:

1. The players take turns.

2. On your turn, you break the array of tiles into two chunks and put them back together in another formation.

3. When a tile has at least two neighbors but none match its color, it blinks with happiness.

4. The first player whose tiles are all happy at once wins.

Fracture illustrates a few features of the system:

1. It would be hard to play Fracture with inanimate pieces because you wouldn't be able to  see at a glance which tiles are happy. You'd have to check all of each tile's neighbors, which would be both onerous and mistake-prone. Automatiles show you when they're happy. They do bookkeeping that would make otherwise impossible games possible.

2. Because the tiles attach and self-align via magnets, the array has a pleasing organization, is easy to manipulate, and hard to knock out of place.

3. The tiles were born of our love for the tactile, social nature of board games, and we designed them to retain that magic. When you play, you don’t feel like you’re playing a video game on a table; you feel like you’re playing a board game that can think.

There are one or two glitchy moments in the video because this is a prototype , but you get the idea.

Note Fracture won't be playable with the base set, which won't have enough tiles for it. Luckily, there are lots of things the tiles can do because of their braaaains:

![automatile-naked.jpg](/uploads/automatile-naked.jpg)

Now we get to design a bunch of games, far and away my favorite thing to do in life (we may also hold a design contest if there's interest) Here are a few ideas:

1. **A "hidden movement" game** (think [Scotland Yard](https://en.wikipedia.org/wiki/Scotland_Yard_(board_game))): there's an AI agent moving around and hiding in the tiles and the players cooperate to find and capture it.

2. **Solo puzzles** where the tiles want to be arranged in some particular configuration, and they glow with anticipation and celebrate their completion.

3. **A flicking game** where you flick tiles across the table with your finger in an attempt to get them to attach in specific ways, and thus trigger events like chain reactions, light shows, etc.

4. **A game that teaches you about color-mixing**. You place tiles of different colors together, and they mix to form the color that you'd get when mixing paint or light. Perhaps your goal is to create some particular color palette before your opponents create theirs.

5. **Each tile is a magic rune**, and each contains its own spell (exerts a unique effects on other tiles). Players take turns casting spells by attaching their runes to a growing array on the table, until some winning condition is reached. Because the system is open source, players could invent, program, and distribute their own runes. There could even be a meta-game economy where players sell the runes they invent.

While we're at it, [here's a poll where you can rank these ideas](https://docs.google.com/forms/d/e/1FAIpQLSf-Cb1Pyuq1FxUHXz_KiL4zICfQlY-6-H-PvLKKPCzfCE1BoQ/viewform) according to how much they appeal to you. We're grateful for feedback.

There's a lot more where that came from. Here's our current stack of game concepts for the system (we're up to 93):

![tile-concepts.JPG](/uploads/tile-concepts.JPG)

That's right, we design with notecards in a wood-paneled room. We don't live in the future ALL the time.

If you're interested in developing games for the system, you can sign up for our developer list [here](http://eepurl.com/cjmjqT).

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