---
layout: post
published: true
title: "Monkey Business #1"
quote: The project idea
image: "/media/MonkeyBusiness1cover.jpg"
video: false
---

## The Project Idea

A common theme for what people do for new projects is to "Build something to scratch your own itch".

So, for the purpose of the project I'm going to build a simple egg timer for hard boiling eggs.

Currently, I repurpose an interval timer app to serve this purpose.  This should be a simple enough application for an introduction to building Android applications with F# so I think that it's a suitable candidate for entry into the Xamarin F# contest.

The way you basically achieve hard boiled eggs (based off of Julia Child's method)

1. Put your eggs into a pot, fill the pot with water up until ~5cm from the top egg.
2. Put the pot on the stove and bring to a boil.
3. Once the water starts to boil, start a timer for three minutes.
4. After three minutes have passed, remove the pot from the stove and leave to cool for 12 minutes (start another timer)
5. Once the 12 minutes is up, rinse the eggs with cold water, peeling the eggs as you go.

The application that I'm going to build should basically walk the user through the above process, the value add is in managing the two timer intervals (boiling time and resting time), prompting the user on each step of the process as you walk through it.

I figure that I'll be needing about 5 screens to run the user through this process, as mocked out as follows:

![2014-07-05 15.19.30_small.jpg](/media/2014-07-05 15.19.30_small.jpg)

![2014-07-05 15.19.34_small.jpg](/media/2014-07-05 15.19.34_small.jpg)

![2014-07-05 15.19.42_small.jpg](/media/2014-07-05 15.19.42_small.jpg)

![2014-07-05 15.19.48_small.jpg](/media/2014-07-05 15.19.48_small.jpg)

![2014-07-05 15.19.53_small.jpg](/media/2014-07-05 15.19.53_small.jpg)
