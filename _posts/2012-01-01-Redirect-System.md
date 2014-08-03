---
layout: post
title: ATD Redirect System
thumb: redirect.png
---

The ATD Redirect System was born soon after we started discussing what we
could do to have an effective lead scoring algorithm at ATD.

We have a pretty sophisticated web analytics implementation but we wanted to
ensure we had an effective way to track incoming links from emails. If we are
promoting an external site that is outside our web properties we can still track
tagging.

Emails are a primary form of communication between ATD and its members
so we devised a system where one could create links and tag them by various
tags.

Each time a customer clicks a redirect link, we make sure to log that into
a SQL Database where we can later report on.

Another very cool result of the redirect system is being able to fix a link
after an email was sent. Since the redirect is stable (we use a Redirect ID)
the target link can be easily fixed without much impact since we opted to use
a 302 redirect.

![Redirect System](/public/redirect-system.png)

Aside from Redirects we can append tons of other information to redirects
including discount, affiliate, and various other codes used for tracking
inbound marketing in tools like Google Analytics and Coremetrics.

The Redirect System still is a huge success. We have over 10,000 redirect
links created and tons and tons of logs (almost 3,000,000 records)
