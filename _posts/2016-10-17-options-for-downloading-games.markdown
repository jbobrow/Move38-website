---
title: When a table game can think for itself, how do you tell it what to do?
date: 2016-10-17 12:00:00 -04:00
tags:
- design
---

Last week we offered [a peek](http://move38.com/blog/a-board-game-that-thinks/) at the game platform we're developing, called AutomaTiles (for now).

![Fracture_hands_01.jpg](/uploads/Fracture_hands_01.jpg)

To recap:

> the game pieces are little computers. They can think, remember, communicate with players and each other, and you can load new games into them. They’re open source so you can invent your own games for them, and they’re easy to program (Arduino!), so they’re also a tool for kids to learn code.

This past weekend, a game designed by [Celia Pearce](http://www.northeastern.edu/camd/gamedesign/people/celia-pearce/), [Mike Lazer-Walker](http://lazerwalker.com/) (his real name / not his Star Wars name) and company was a finalist at [IndieCade](http://www.indiecade.com/). For 3 days, Jonathan watched hundreds up people play, in the words of Mike, "a futuristic cyber chess".

<iframe width="720" height="405" src="https://www.youtube.com/embed/6Dg2JGaZMSk" frameborder="0" allowfullscreen></iframe>

In keeping with our open philosophy, today I'm discussing a design issue we're facing. We hope you'll read it and offer your opinion. It has to do with this bit:

> you can load new games into them

The question is: how?

Right now, you load games into the tiles one-by-one, by removing their covers and getting into the hardware, like this:

![IMG_0992.JPG](/uploads/IMG_0992.JPG)

...which is fine for tinkerers and programmers but not for people who just want to play games. We've learned 6-12 year olds are crazy in love with the tiles, so switching games must be easy even for them.

We need a loading method with the following characteristics:

1. downloading a game should happen at the press of a button

2. the user shouldn't have to load tiles one-by-one.

3. downloading shouldn't require taking the tiles apart

We have two options which meet these criteria, but we haven't decided which to implement:

## option #1 - download from phone via Bluetooth

One of the tiles will communicate with your phone by Bluetooth, and there'll be an app that comes with the tiles. When you want to play a new game, you open the app and select the game you want to play. The phone zaps the instructions to the tile with Bluetooth, and when that tile is attached to all the other tiles, it sends instructions to them via their normal communication (infrared)

## option #2  - games on tiles

Each tile will come with a game preprogrammed on it. When you want to play a new game, you attach the tile with the game you want to all the other tiles and hold and press its top. It then sends instructions to all the other tiles.

Here are the strengths and weaknesses of these options as we now understand them:

![Screen Shot 2016-10-17 at 8.56.44 AM.png](/uploads/Screen%20Shot%202016-10-17%20at%208.56.44%20AM.png)

But we're not sure we fully understand the parameters of the problem yet. If you have a preference for one of these options, or know of strengths or weaknesses we've missed, let us know in the comments. That's our entire reason for posting this. We want to suck the knowledge from your succulent brain and leave it a desiccated, ignorant husk.

## one last thing

We're looking for electrical engineers to join our team.

If you or someone you know is one, likes where we're headed, and gets the process of building open source hardware (i.e. Arduino), contact jobs@move38.com

If you'd like to follow our work (and be alerted when our games launch), sign up here:

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
