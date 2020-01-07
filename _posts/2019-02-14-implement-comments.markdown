---
layout: post
title:  "Implement comments"
date:   2018-11-11 04:04:00 -0600
categories: jekyll update
comments: true
---

# Implementing comments

 * To implement comments on my blog I used [Disqus to create my account](https://disqus.com/).
 * Start by filling in the details to set up your account.
 * Do not forget to set `comments: true` in your post-layouts YAML Front Matter.
 * You will be given a universal code to implement to your site. I had to change `this.page.url` and `this.page.identifier` as shown below, only to work when I filled in the url-variable in my `_config.yml`.
 * `YOUR_WEBSITE_NAME` you also have to change, it is your disqus-username, don't be like me and missspell it :)

 ```
{% if page.comments != false and jekyll.environment == "production" %}

  <div id="disqus_thread"></div>
  <script>
    var disqus_config = function () {
      this.page.url = '{{ page.url | absolute_url }}';
      this.page.identifier = '{{ page.url | absolute_url }}';
    };

    (function() {
      var d = document, s = d.createElement('script');

      s.src = 'https://YOUR_WEBSITE_NAME.disqus.com/embed.js';

      s.setAttribute('data-timestamp', +new Date());
      (d.head || d.body).appendChild(s);
    })();
  </script>
  <noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>
{% endif %}

 ```