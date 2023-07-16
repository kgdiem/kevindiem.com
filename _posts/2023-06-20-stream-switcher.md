---
layout: post
date: 2023-06-20
title: StreamSwitcher
description: Launching my first App Store App
image:
---

## TL;DR

I made an app! The App Store submission process can seem daunting at times but ChatGPT and Midjourney can come in handy.

## Inspiration

Around Christmas of last year I met a lady and almost immediately we began sending songs back and forth. The only problem was that I use Apple Music and she uses Spotify.

That meant I had to either listen to a short preview on the Spotify web client or open Apple Music and search for it and she had to open Spotify to find my Apple Music links.

This was a scenario I've faced for a long time as a member of the less popular music streaming service. Any time I'd send a song to someone I'd have serious doubts that they'd ever open it but 🤷; it's the thought that counts, right?

## The Easy Part

Making StreamSwitcher was actually a really pleasant and enjoyable experience.

I had off of work on the day before New Year's Eve and decided that I might as well make an app.
After 8 or 9 hours stumbling around in XCode I had a working PoC.

I spent an hour or two refining a couple of weeks later and **boom**, StreamSwitcher was done.
I had a crappy icon I drew up in Seashore so it definitely wasn't read for release but I was able to send the app to TestFlight to have some people test it out.

## The Daunting Part

I'd completed the app in early January 2023 and finally got around to generating an appealing icon with Midjourney in April. It was pretty actually pretty fun to generate a bunch of different icons and I am pretty proud of the result.

Around the same time I generated the app icon I figured I'd get going with the App Store listing.
StreamSwitcher is free and doesn't collect any user data so a privacy policy wasn't someting I was interested in paying for.
With a little googling I found an awesome tool, [App Privacy Policy Generator](https://app-privacy-policy-generator.nisrulz.com/), to generate the terms of service and privacy policy. Thanks Nishant!

### Getting Close

After I generated the icon and policies I was still dreading making a marketing site, a contact form and the like so I put it off.
Just a week or so ago I reasoned that I might as well start publishing the work I actually finish so [I started looking into Jekyll](https://www.kevindiem.com/2023/06/19/first-post.html) after remembering my good friend [Stanley](https://github.com/ST215) had used it extensively in the past to good effect.

All that was left was the App Store marketing copy and some screenshots, easy enough right? Well, the copy was easy enough. My buddy [Jake](https://github.com/jdiffy47) has been using ChatGPT to make marketing copy for a bunch of sites he's been creating so I figured I might as well do the same. Took about 15 minutes to get something workable and touch it up a bit.

### Screenshots: The Simulator Offers No Hope

I have a newish iPhone without a home button, 12, 13, something like that. I figured it'd had to be the standard so I went about making a couple of fun ~videos~, err..., _app previews_ and bugged some friends with what must have seemed like delusional texts without any context and thought everything was swell until I logged into App Store Connect.

My iPhone isn't the right screen size! I have a 6.1" screen and the required screenshot size is 6.5". Luckily the aspect ratio is the same so I was able to stretch my 6.1" screenshots in Photoshop without much fuss.

It was even more of a surprise that I needed to take screenshots on a **5.5"** iPhone and 2 kinds of 12.9" iPads. Ordinarily that wouldn't pose much of a challenge, that's what the Simulator is for, but StreamSwitcher necessarily uses MusicKit for 50% of the app's functionality -- showing your recently played songs in Apple Music -- and MusicKit doesn't work in device simulators.

I checked with everyone I could think of that'd be willing and able to install the app through TestFlight on a Saturday morning and not a single person had an iPhone 8 Plus, 7 Plus or a gigantic iPad so I had to settle with using the simulator if I wanted to get the app submitted for review and stop putting it on the backburner.

### Screenshots Episode 2: Apple Strikes Back

I submitted the app to the App Store on Saturday, 6/17 and it stayed in the queue until Monday, 6/19 which is fair enough. It wasn't until the morning of Tuesday, 6/20, that I got the bad news: my app was rejected because I used copyrighted images in the screenshots.

Midjourney saved the day again, though, because I was able to generate a bunch of fake album art and replace the album art in the screenshots in a relatively short period of time and resubmit the app for review.

It wasn't a complete win though because I had to remove my app previews.

## What's Next?

### More Features

Adding support for Spotify to Apple Music! I completed the selfless half of the equation of the streaming conondrum by enabling Apple Music users to quickly sending Apple Music songs as Spotify links to their friends.

Sending from Spotify to Apple Music requires just a bit more effort because I'll have add an OAuth Client for Spotify and likely create an app
to go along with the message extension.

### SwiftUI

XCode generates a new message extension project with Storyboards. I'd used storyboards several times over the years to make some unreleaed iOS
apps so I was comfortable enough getting started.

Since I'd made StreamSwitcher I'd since tried out SwiftUI and I was impressed to say the least. The visual element of Storyboards is nice but
the data-binding, state, observables and overall declarative nature of the code when creating views makes me think I am going to enjoy making iOS apps much more going forward

### A Gigantic iPad

I started looking on eBay for a bottom tier, 2nd gen 12.9" iPad Pro. I imagine it'll sit around with my Android dev phones and tablets but hopefully it'll keep getting iOS updates for longer than they did.
