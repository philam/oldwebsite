---
id: 3624
title: 'A farewell to Wordpress'
date: '2024-03-02T21:02:21+11:00'
author: Philip
image: https://raw.githubusercontent.com/jekyll/brand/master/jekyll-logo-dark-solid.png
categories:
    - Meta
tags:
    - Meta
---

It's hard to say goodbye sometimes.

I have been running a personal website since my council election campaign 14 years ago in February 2012. I started on WordPress at the time - back in <a href="https://wordpress.org/documentation/wordpress-version/version-3-3/">Version 3.3</a> when it looked like this:

![Screenshot of a dashboard of Wordpress 3.3](/images/posts/wordpress-3-3-2.jpg)

As a non-developer this was a steep learning curve at the time. I knew nothing about DNS, web hosting or HTML. Over these years I have slowly taught myself some basic skills; although I'd say that I'm still very much a novice.

After all this time I recently decided that it was time for a change.

The reasons for this are partly because WordPress has changed and partly because I want to try something new.

For a personal website where the main aim is to present information and host blog posts, WordPress is now overkill. At the time when I started in 2012 it was ''the'' place to start. It was easy to set up, lightweight and a breeze to write.

Now I find it too bloated and even slightly annoying to use. Its installation is still very easy and it deserves a lot of credit. But the Gutenberg Editor has never really grown on me and I found that I was having to stack more and more plugins on top of each other to get my website to do what I wanted.

And so I started researching alternatives in late 2023 which eventually led me to find <a href="https://jekyllrb.com/">Jekyll</a>.

It's a static site generator that has been around for a while and is lightweight.

These two factors are the main ones that attracted me. Ideally I do not want a database to host a basic website and a long history also means a higher likelihood of a strong user base and better documentation.

This isn't to say that Jekyll is necessarily the best answer for what I want. It's just the one that I have gone with because I have found it the easiest to get my head around. Even then there are still things that I don't fully understand or have spent a long time trying to figure out.

I am hosting Jekyll on <a href="https://pages.github.com/">Github Pages</a>. This is proving complicated because the theme here relies on Gems and dependencies that Github does not natively support in Safe Mode. This means there is a workaround using Github Actions and some other <a href="https://github.com/CloudCannon/vonge-jekyll-bookshop-template/issues/22">tenuous trickery</a> that works but in a very roundabout way. I'm not very happy with it and hopefully a better solution comes up.

For completeness I am using:

<ul>
    <li><a href="https://remark42.com/">Remark42</a> for the comments system (if I can get the import function to work)</li>
    <li><a href="https://www.mailerlite.com/">Mailerlite</a> for my newsletter</li>
    <li><a href="https://www.zoho.com/forms/">Zoho Forms</a> for the contact form.</li>
</ul>

Some things may be a bit broken as this transition is complete. It's hard to move a website that's operated using the same software for 12 years. But hopefully it will all be worth it.

It's entirely possible that I switch software again as I use Jekyll more, or even switch back to WordPress.  Ghost, Hugo and Publii were all contenders at various points.

I'm only interested in something that works and doesn't require a lot of maintenance or pain to change or use the site. I will happily switch again if needed.

It has been quite an adventure.
