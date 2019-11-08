---
layout: post
title: 'JS Applet to Kill Popups'
---

{{ page.title }}
================

<p class="meta">Code</p>

### JS Applet to Kill Popups

With a lot of businesses only operating in the digital space these days, more importance of connecting with their content-consumers(readers), users, and potential customers these days is involved and has a lot of depth. A significant thing I seem to hear a lot for digital marketers is collecting emails; if you're not doing that in 2019, you're apparently doing it wrong. Most of the idea of digital marketings depth seems to shift the web into a landscape of websites that have the same element and what we all thought was a thing of the past: Pop-ups.

Some digital business do it well and embedd the email sign-ups along their content and not as an overlay, but other websites immediately throw a popup at you explicitly asking for that email. It's annoying enough since GDPR passed, the mandatory additional box asking you to accept their terms of tracking_agreement. These emails collected are used in the hopes they can funnel you into their drip campaigns and annoy the shit out of you, until you feel so hopeless that you buy their xyz. If pop-ups weren't involved I wouldn't be so negative here. You should be collecting emails, but if you have a pop-up to do it, I'm going to find a way to break it.

And that is what this post is about. I'm here to help you get rid of the popup with an JS Applet that I found on the web and has served me well in avoiding the new norm of website pop-up blocks.

### Expanding

Javascript applets are little pieces of javascript that can do everything from modify a website you’re on in a variety of ways, with this we're going to kill anything that floats above the content.

- Open a New Tab in Chrome. Command+T on a Mac, Ctrl+T on a Windows.
- Right click on the Bookmarks Toolbar.
- Select “Add Page” from the contextual menu that appears.
- Give the Bookmark a name, I've called mine -popup.
- Paste the Javascript applet into the URL field.
- Save.

Applet Code:
```
javascript:(function()%7B(function()%7Bdocument.body.style.overflow %3D 'auto'%3B(function () %7Bvar i%2C elements %3D document.querySelectorAll('body *')%3Bfor (i %3D 0%3B i < elements.length%3B i%2B%2B) %7Bif (getComputedStyle(elements%5Bi%5D).position %3D%3D%3D 'fixed') %7Belements%5Bi%5D.parentNode.removeChild(elements%5Bi%5D)%3B%7D%7D%7D)()%7D)()%7D)()
```

Next, I want you to find a website that bugs you. After you visit it, write down from 1-10 pain rating of your experience. Or really, just when the pop-up shows up all you have to do is click the Applet you just created and it should remove the overlays on the page. 

Note: it's not permanant and yes, sometimes it has adverse affects, like removing the navigation bar or some other overlaying elements on the page that aren't the target. Regardless, it has a lot of uses and this is just one of them, I reccomend playing around with it, if it removes an element that you didn't intend to remove, just refresh the page and endure the overlays.
