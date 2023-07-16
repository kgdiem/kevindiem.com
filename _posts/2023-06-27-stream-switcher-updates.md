---
layout: post
date: 2023-06-27
title: StreamSwitcher Updates
description: Spotify => Apple Music Support & setting the stage for the long-delayed LTThis App and the StreamSwitcher API
image:
---

## TL;DR

StreamSwitcher is creating a map of links from Spotify to Apple Music that will power the StreamSwitcher API and a collaborative, cross-platform playlist app. Also, Spotify => Apple Music support is on the StreamSwitcher roadmap!

## Motivation

[As previously mentioned](https://kevindiem.com/2023/06/19/first-post.html) I'm committed to privacy and anonymity online. StreamSwitcher is free and will never display ads or collect user data.

StreamSwitcher is intended to provide utility to the end user -- enabling a seamless share experience with people who use a different streaming service.

In turn, the users are providing me with the correct mapping of an Apple Music link to a Spotify link.

This creates a mutually beneficial arrangement where I'm getting data I need for other projects and users are able to share the content they want, opening a path towards alternative forms of monetization.

## Implementation

When a user selects a recently played song from Apple Music, a session ID is generated and the URL of the Apple Music song is recorded along with that sesison ID.

If the user selects a song from Spotify, the session ID and spotify link are recorded. If the user instead cancels the search, the session ID is cleared and a new one will be generated next time they click.

I don't use any device identifier, IP address, or other form of identifiable information from the end-user. Each session is completely anonymous.

## What's Next

### Spotify Support

Before I put effort into promoting the StreamSwitcher iOS app I want to add Spotify => Apple Music support to expand the potential audience. Thusly I will be working to add a full fledged app (as opposed to just an iMessage Extension) to choose the platform you use and perform OAuth with Spotify if necessary.

### StreamSwitcher API

Given the mapping of songs being created by the StreamSwitcher app I plan to create an API that converts song links from Apple Music to Spotify or vice-versa.

This will be a paid service with TBD pricing.

### LTThis App

Over a year ago a friend of mine asked about making a playlist app for the [Listen To This Subreddit](https://www.reddit.com/r/listentothis/) and I liked the idea so I got to working on it.

I got to the point of creating a pipeline that loads posts from the beginning of the Reddit, normalizes them, and searches Apple Music and Spotify for the link to the song in their respective apps.

It also has an admin UI that allows you to create a playlist by genre, artist, etc then save it in your Spotify or Apple Music account.

I'd run into some issues with the dead letter queue and never circled back to fixing the pipe or getting it ready for release.

I'm aiming to revive portions of the LTThis App to create a cross-platform, collaborative playlist builder.

This app will have a free tier and a subscription tier at ~ $1.99/mo or $9.99/year and will utilize the StreamSwitcher API.
