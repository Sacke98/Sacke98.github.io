---
layout: post
title:  "Open graph"
date:   2018-11-11 04:04:00 -0600
categories: jekyll update
comments: true
---

# What is Open Graph and how do you make use of it?

Open Graph is a way for developers to define what content is going to be presented when the page is shared on social media. 
Bacically when someone sends a url on your webpage a selected picture is shown with a choosen descripsion. 

To create this you need to put meta-tags in the header and fill with wanted informatiom.
You also need atleast 4 required properties for every page. What is shown below is how I implemented my meta-tags in my header.
There are some optional also, depending on what will suit your site. 

# Optional metadata

og:audio - A URL to an audio file to accompany this object.
og:description - A one to two sentence description of your object.
og:site_name - If your object is part of a larger web site, the name which should be displayed for the overall site. e.g., "IMDb".
og:video - A URL to a video file that complements this object.

# How I did it

```
"<head>
<meta property="og:title" content="Sakibas Blogg" />
<meta property="og:type" content="website" />
<meta property="og:url" content="https://Sacke98.github.io" />
<meta property="og:image" content="/assets/img/01.jpg" />
</head>"
```