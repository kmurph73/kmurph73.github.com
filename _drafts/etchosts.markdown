---
layout: post
title:  "Blocking Sites"
permalink: /etchosts
date:   2016-06-05 10:00:00
categories: productivity
---

Like many, I struggle with the many digital distractions.  Opening the browser and typing 'reddit' is burned into my fingertips.  Before I know it, 30 minutes of web browsing will pass.

In the past, I've used the [StayFocusd][1] chrome extension, which, while a massive improvement over nothing, was still too easy to circumvent by switching browsers, or switching Chrome users.

Enter the [hosts][2] file, which on OS X & Linux can be found in /etc/hosts.  It allows you to map domains to an ip address, which can be effectively utilized to block distracting sites.

`127.0.0.1 www.reddit.com`  Will map Reddit to your local machine's address, i.e. nowhere.

The problem with this is it can be a bit of a pain to type `sudo mvim /etc/hosts` then (un)comment out the sites then save & quit.

[1]: https://chrome.google.com/webstore/detail/stayfocusd/laankejkbhbdhmipfmgcngdelahlfoji?hl=en
[2]: https://en.wikipedia.org/wiki/Hosts_(file)
