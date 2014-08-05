---
layout: post
title: ATD Lead Scoring Algorithm
thumb: lead-score.png
---
We decided to create a lead scoring algorithm to be able to deliver relevant
content to our customers.

Me and some other ATD folks sat on a room and decided that - at a minimum -
we should be able to attribute lead score points to:

* **Orders**: each of our products are mapped to our areas of interest.

* **Web site visits**: we published a ton of blogs, articles and newsletters.

* **Emails**: emails are still a big part of how we communicate
with our members. We need to take in consideration the items they click on
to understand what are their interests.


To have that information we had to put a lot of things in place, between
tagging content effectively, using web analytics to all it's potential, and creating
systems that would allow us to track things such as email link clicks.

Once the data collection started, we created a function
that assigns a point for each of those activities. We also added a decay factor
to each of them so a "Web Article Point" today is worth "1" but a year ago it is worth 0.02, as an example.

Finally, we are 'flattening' these lead scores (having 50, 100, 1000) points might be the same when 'interest' is concerned. So we wanted to stay with a 0-100 range.

At ATD we have over 10 lead score fields per customer.

We use this information to target ads on our site, recommended products and a lot
of other things.
