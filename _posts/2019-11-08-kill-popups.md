---
layout: post
title: JS Bookmarklet to Kill Pop-up Overlays
---

{{ page.title }}
================
<p class="meta">Code, Bookmarklet, Tutorial, Utility, Marketing</p>

![Pop-up Hero](/images/-popup-hero.jpg "Free, Just enter your bank info!")

### What's the big deal? Expanding on what's going on, and why this might be useful.

With a lot of businesses only operating in the digital space these days, more importance of connecting with their content-consumers(readers), users, and potential customers these days is involved and has a lot of depth. A significant thing I seem to hear a lot for digital marketers is collecting emails; if you're not doing that in 2019, you're apparently doing it wrong. Most of the idea of digital marketing's depth seems to shift the web into a landscape of websites that have the same element and what we all thought was a thing of the past: Pop-ups.

Some digital business do it well and embed the email sign-ups along their content and not as an overlay, but other websites immediately throw a popup at you explicitly asking for that email. It's annoying enough since GDPR passed, the mandatory additional box asking you to accept their terms of tracking_agreement. 

These emails collected are used in the hopes they can funnel you into their drip campaigns and annoy the shit out of you. If pop-up overlays weren't involved I wouldn't be so negative here; You should be collecting emails, but if you have an overlay to do it, I'm going to find a way to break it. Also, when I'm reading a news article and a navbar on the bottom and the top of the page obstructs my view from the text, it's plain frustrating!

> You should “own” your audience contact details, rather than optimise for followers on proprietary networks that you need to continually pay to reach.

And that is what this post is about. I'm here to help you get rid of the popup with an JS Bookmarklet that I found on the web and has served me well in avoiding the new norm of website pop-up blocks.

### Explaining how to create an bookmarklet, and in this case kill pop-up overlays

Javascript Bookmarklet are little pieces of JavaScript that can do everything like modify a website you're on in a variety of ways. In this case, we're going to kill anything that floats above the content.

### Create Bookmarklet(clickable bookmark)

- Open a New Tab in Chrome. Command+T on a Mac, Ctrl+T on a Windows.
- Right click on the Bookmarks Toolbar.
- Select "Add Page" from the contextual menu that appears.
- Give the Bookmark a name, I've called mine `-popup`.
- Paste the Javascript Bookmarklet into the URL field.
- Save.

### Bookmarklet Code:
```
JavaScript:(function()%7B(function()%7Bdocument.body.style.overflow %3D 'auto'%3B(function () %7Bvar i%2C elements %3D document.querySelectorAll('body *')%3Bfor (i %3D 0%3B i < elements.length%3B i%2B%2B) %7Bif (getComputedStyle(elements%5Bi%5D).position %3D%3D%3D 'fixed') %7Belements%5Bi%5D.parentNode.removeChild(elements%5Bi%5D)%3B%7D%7D%7D)()%7D)()%7D)()
```

![You can also create this by editing a bookmark and add the code like this](/images/-popups.png "Popup Bookmarklet Alt-Creation: You can also create this by editing a bookmark and add the code like this")

Next, find a website that bugs you. Write down using a scale from 1 to 10, your pain rating of your experience... or really, just when the overlay shows, just click the Bookmarklet you've just created. It should remove the pop-ups and overlays on the page, no more clutter.

_Note: If you used the Bookmarklet and it removed elements, you didn't want removed -- don't worry! Just refresh. It's not permanent. But yes, sometimes it has adverse affects, like removing the navigation bar or some other overlaying elements on the page that aren't your target. Regardless, it has a lot of uses and this is just one of them, I reccomend playing around with it, if it removes an element that you didn't intend to remove, again, just refresh the page and endure the overlays._

![Blammmo](/images/blam.gif "
Pop-ups get Blam'd")
