---
layout: post
date: 2023-06-19
title: Inaugural Post
description: Launching a Blog on a Budget; Using Jekyll, S3 and Cloudflare to revamp my personal site, start a blog, and create an app landing page.
image:
---

## TL;DR

Launching a blog on a budget: Using Jekyll and S3 to revamp my personal site, start a blog, and create an app landing page.

## Portfolio Sites

When I started learning about web development in a serious way and completed [Free Code Camp](https://freecodecamp.com) I'd hand-written several different portfolio sites. As I started working full time and continued to hack on projects the last thing I wanted to do was write HTML and CSS for a portfolio site.

When I felt the need to keep a web presence without any maintenance I'd used Wix, which as of this writing is $16/mo not including a domain name. For a long time I went without a webpage. Then, not too long ago, I coded up a quick template on Codepen and started hosting a static site via S3. Including the annual domain fee, I'm able to host my static site for less than $2/mo.

## Blogging

Over the years I've made a few blog posts on Steemit and was asked to write an entry on the CosmicJS blog for my [Cosmic Contentful Importer Extension](https://www.cosmicjs.com/changelog/creating-the-cosmic-js-contentful-importer-k5qwyunz). It's something I've always wanted to do more of and thanks to [Jekyll](https://jekyllrb.com/) I'm able to do it really easily and for free on my own domain. Many thanks to [Andrew Banchich](https://github.com/andrewbanchich) for this [awesome theme](https://github.com/andrewbanchich/forty-jekyll-theme).

## Enter StreamSwitcher

The driving motivation for getting started with Jekyll is my first iOS app, Stream Switcher. I've launched at least 4 Android Apps, it's been a long time so it's a bit blurry. The App Store submission process is much more involved than it's more playful counterpart. I needed a website, a contact form, a privacy policy, terms and conditions, not to mention lots of screenshots for different devices.

I figured I could use Wix, GoDaddy, etc. but there are a few problems with that:

1. StreamSwitcher is 100% free; there are no ads, no data harvesting and no plans to monetize
2. I have plans to launch a low cost data service imminitely
3. I am very much looking forward to creating more iOS apps with minimal monetization (eg low price subscriptions, $0.99 - $2.99 apps).

With free and hobby projects that _might_ generate a few bucks a month it's senseless to throw $15/month away for every site I might want to make.

With Jekyll, S3 and Cloudflare I'm free to throw as many subdomains or nested folders into an bucket and have a site up in a few minutes and hosting will rarely, if ever, exceed $1-2/month.

## Going Forward

Recently I've been exploring **doing more with less**, especially preferring utilizing database features over code running on servers (think postgres triggers instead of lambdas, sprocs and UDFs instead of ETL-in-code).

I'm also extremely interested in alternative paths to software monetization, decentralization, and creating great user experiences while respecting privacy and end-user-autonomy.
