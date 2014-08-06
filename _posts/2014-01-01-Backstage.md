---
layout: post
title:  Backstage
thumb:  backstage.png
---
The idea behind Backstage was to create an aggregated page
of tweets and information about a certain hashtag.

Perfect uses for my Twitter aggregation tool include conferences and sporting events like Winbledon or the US Open, for exemple.

Backstage used a [node.js](http://nodejs.org) module to connect to the [Twitter Streaming API](https://dev.twitter.com/docs/api/streaming).

Every time a certain tweet matched its configured hashtag, Backstage would:

* Save the data into a no-sql (MongoDB) database
* Extract links, videos, pictures
* Extract titles, descriptions and thumbnail (I used [Cheerio](https://github.com/cheeriojs/cheerio) to accomplish this)

My goals for Backstage:

* To list the most popular tweets on a topic
* To list popular media items associated with that hashtag (videos, images)
* To list popular articles and URLs shared (with their meta-data)
* To provide a curated list of who to follow (and popular tweets from them). These could be players or SMEs.
* To promote the topic even further by effectively using colors, images (think css, background images, etc.)

I still think the idea is great but haven't had time to push it further into development.
