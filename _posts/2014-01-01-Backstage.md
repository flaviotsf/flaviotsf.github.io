---
layout: post
title: Twitter Backstage
thumb: backstage.png
---
The idea behind Twitter backstage was to create an aggregated page
of tweets and information about a certain hashtag.

Perfect fits are conferences or sporting events like Winbledon or the US Open, for exemple.

Backstage used a [node.js](http://nodejs.org) module to connect to the [Twitter Streaming API](https://dev.twitter.com/docs/api/streaming).
Every time a certain tweet matched my watched hashtag, Backstage woud:

* Save the data into a no-sql (MongoDB) database
* Run a few other processes. I was extracting links as well so I could
build a 'top list' of links shared. To do that, I used Cheerio to extract titles, descriptions and thumbnail images
from the links that were being shared.

The goal of Backstage was to have:

* List of most popular tweets on that topic
* List of media items associated with that hashtag (videos, images)
* Curated list by the organizer of the hashtag of who to follow (and tweets about those folks)
* A branded landing page that pushed the hashtag even further.


I still think the idea is great but haven't had time to push it further
into development.
