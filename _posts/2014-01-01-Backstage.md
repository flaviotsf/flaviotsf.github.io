---
layout: post
title:  Backstage
thumb:  backstage.png
---
The idea behind Backstage was to create an aggregated page
of tweets and information about a certain hashtag.

Perfect fits are conferences or sporting events like Winbledon or the US Open, for exemple.

Backstage used a [node.js](http://nodejs.org) module to connect to the [Twitter Streaming API](https://dev.twitter.com/docs/api/streaming).

Every time a certain tweet matched its configured hashtag, Backstage would:

* Save the data into a no-sql (MongoDB) database
 Run a few other processes. I
* was extracting links as well so I could
 build a 'top list' of links shared.
* To do that, I used [Cheerio](https://github.com/cheeriojs/cheerio) to extract titles, descriptions and thumbnail
* images
 from the links that were being shared.

My goals for Backstage:

* List of most popular tweets on a topic
* List of popular media items associated with that hashtag (videos, images)
* List of popular articles and URLs shared (with their meta-data)
* Curated list of who to follow (and popular tweets from them)
* A branded landing page that pushed the hashtag even further (think CSS, background, etc.)

I still think the idea is great but haven't had time to push it further
into development.
