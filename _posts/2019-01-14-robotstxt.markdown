---
layout: post
title:  "Robots.txt"
date:   2019-01-14 04:04:00 -0600
categories: jekyll update
comments: true
---

# What is robots.txt and how have you configure it for your site?

Web site owners use the robots.txt file to give instructions about their site to web robots.
Imagine a robot wants to visit a Web-URL, the first thing it does is to check for i.e http://www.example.com/robots.txt and finds directions on what parts it is allowed and likely others it is not to visit. 

```
User-agent: *  this means that it applies to all robots
Disallow: /   Tells the robots that it should not visit any pages on the site


Disallow:     medger full tillgång
Disallow: /...../
```

However, there are two important conciderations when using robots.txt:
* robots can ignore your /robots.txt file, especially malwere. Robots that scan the web for security vulnerbilities, and email adress harvesters used by spammers will pay no attention. 

* The /robots.txt file is publicly available file. Anyone can se what sections of your server you don't want robots to use.

* While creating your file you should locate it in the top level directory of your web server.