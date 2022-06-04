---
layout: post
title: Using Stylus, a Browser Extension
---

{{ page.title }}
================
<!--Available Meta Tags: CSS, Code, Applet, Tutorial, Utility, Design, Extensions, Marketing -->
<p class="meta">CSS, Tutorial, Code, Utility, Design, Extensions</p>

![Stylus Hero](/images/-stylus-hero.jpg "I love this team, but what is their mascot?")

### What is Stylus?

Stylus is an extension for your browser where it can allow you to edit the visual styling of websites. It also has a lot of styles for download other users created which you can find by clicking Find styles. A similiar extension that a lot used to use was Stylish[[0]](https://robertheaton.com/2018/08/16/stylish-is-back-and-you-still-shouldnt-use-it/)[[1]](https://arstechnica.com/information-technology/2018/07/stylish-extension-with-2m-downloads-banished-for-tracking-every-site-visit/), but that was found to be tracking users and ultimately killed.

Anyways this is a rundown on how to get started and how you could use Stylus. Maybe you want a Dark Theme for HackerNews? What about moving some element on a website you use to make it easier to navigate through? _Create your own prefered user experience._

---

##### Download:
- [Chrome:](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne?hl=en) 
https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne
- [Firefox:](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)
https://addons.mozilla.org/en-US/firefox/addon/styl-us/

<HR>

### Using Stylus
Once the extension is added to your browser, left click the icon. You have a couple options, _Turning all styles off_, _Finding styles_ other users created, a button for _inline_ to display the results of the previous: finding styles, then _write styles_ for this, and a link to the _current page_, as well as buttons for _manage_, _options_, and _wiki_.

The ones I frequently use is, turning off all styles: to toggle edits that I've made to see how I could improve them better without getting distracted by the current edits. And also the link that says _Write Styles for:_ The cool thing about this link below this is that it is hoverable, you can hover the far right and it will create a style for the current page: _this URL_. Otherwise, you can click the begining part of the link and create a global style for the entire website. When deciding which one is better for you, first figure out what you want to do and how it might effect the other parts of the website that you might use all the time.


### In Use
Use stylus to edit the pages you're seeing errors in Google Dev tools. While you're actively tweaking things, think of Stylus as a way to save what you're editing in Dev tools; do this to see changes live without having to save it to your server, then wait for your style.css cache to refresh. This is much faster and here is a small example, of something I did using this post.

![Stylus Example](/images/stylus-example.gif "Change colors, without having to remember hex codes, everything you can do with CSS it is easier with Stylus")

_**Above:** As you can see, the `.site` class in my CSS was showing `min-width: 50vw` and skewing columns when the site was a little smaller. So in this case, I used it to edit this down on the fly and make sure if you had a smaller browser, then the site wouldn't look totally messed up. To fix this, I removed the `min-width` and made it the max-width, then set the min-width to something I was comfortable with visually. All without having to save the style.css and refresh the site to see if it's where I want it. In the future I plan on posting about some of the popular sites edits that I use, and make some of the sites more enjoyable._

_Play around with Stylus and email me if you think you have a cool style for a website that I might enjoy!_
