---
layout: post
title:  "A Post with a Video"
date:   2018-11-03
excerpt: "Custom written post descriptions are the way to go... if you're not lazy."
tag:
- sample
- post
- video
comments: true
---
<center><iframe width="560" height="315" src="//www.runoob.com/try/demo_source/mov_bbb.mp4" frameborder="0"> </iframe></center>

Video embeds are responsive and scale with the width of the main content block with the help of [FitVids](http://fitvidsjs.com/).

Not sure if this only effects Kramdown or if it's an issue with Markdown in general. But adding YouTube video embeds causes errors when building your Jekyll site. To fix add a space between the `<iframe>` tags and remove `allowfullscreen`. Example below:

{% highlight html %}
<iframe width="560" height="315" src="//www.runoob.com/try/demo_source/mov_bbb.mp4" frameborder="0"> </iframe>

{% endhighlight %}