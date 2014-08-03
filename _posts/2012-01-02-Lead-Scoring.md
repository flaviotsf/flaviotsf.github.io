---
layout: post
title: ATD Lead Scoring Algorithm
thumb: lead-score.png
---
We decided to create a lead scoring algorithm to be able to deliver relevant
content to our customers.

Me and some other ATD folks sat on a room and decided that - at a minimum -
we should be able to attribute lead score points to:

* **Orders**: each of our products are mapped to our areas of interest. We should
be able to use that information to know what a customer is interested in.

* **Web site visits**: we published a ton of blogs, articles and newsletters. Those
are also some great data points.

* **Emails**: emails are still a big part of how we communicate
with our members. We need to take in consideration the items they click on
to understand what are their interests.


To have that information we had to put a lot of things in place, between
tagging content effectively, used web analytics to all it's pontential and creating
systems that would allow us to track things such as email link clicks.

We waited a few weeks for this data to start to populate and created a function
that assings a point for each of those activities. We also added a decay factor
to each of them so a "Web Article Point" today is worth "1" but a year ago it will
be worth 0.02, for example.

We also decided to 'flatten' the point structure a bit (having 50, 100, 1000) points
might be the same when 'interest' is concerned. So we wanted to stay with a 0-100 range.

At ATD we have over 10 lead score fields. One for each of our content areas.

We use this information to target ads on our site, recommended products and a lot
of other things!
