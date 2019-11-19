---
layout: post
title:  "Open graph"
date:   2018-11-11 04:04:00 -0600
categories: jekyll update
comments: true
---

# What is Open Graph and how do you make you of it?

Open Graph is a way for developers to define what content is going to be presented when the page is shared on social media. 
Bacically when someone sends a url on your webpage a selected picture is shown with a choosen descripsion. 

To create this you need to put meta-tags in the header and fill with wanted informatiom.
You also need atleast 4 required properties for every page.

```
"<head>
<meta property="og:title" content="Sakibas Blogg" />
<meta property="og:type" content="website" />
<meta property="og:url" content="http://www.imdb.com/title/tt0117500/" />
<meta property="og:image" content="http://ia.media-imdb.com/images/rock.jpg9" />
</head>"
```