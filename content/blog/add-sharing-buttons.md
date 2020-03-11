+++
date = "2016-04-15"
draft = false
title = "add sharing buttons"

+++

this is becoming my official personal blog and I'm inclined to post some quality content here.
so I better add some sharing buttons.
but how does one do this in Hugo?

I recalled I had a [Shareaholic] (https://shareaholic.com/) account I've used before. Shareaholic is free and very easy to set up.

I've generated the code snippets from their control interface and pasted them to my theme's layout html files (I'm using the wonderfully minimal [cocoa theme](https://github.com/nishanths/cocoa-hugo-theme)):

in themes/cocoa/layouts/partials/head.html :
{{< highlight html >}}
<script type='text/javascript' src='//my.shareaholic.url/assets/pub/shareaholic.js' data-shr-siteid='4c511..e8c' data-cfasync='false' async='async'></script>
{{< /highlight >}}
and in themes/cocoa/layouts/blog/single.html :
{{< highlight html >}}
<br>
<div class='shareaholic-canvas' data-app='share_buttons' data-app-id='somenumberfromshareaholic'></div>
<div class="disqus">
{{< /highlight >}}
Voila - the sharing buttons are right here below this post. Sharing makes you richer!
