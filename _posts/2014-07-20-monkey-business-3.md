---
layout: post
published: true
title: "Monkey Business #3"
quote: Xamarin and F# Project Debriefing
image: "/media/MonkeyBusiness3cover.jpg"
video: false
---
## Project Debrief

I thought I'd do a debrief of this project to recap on what went well, what was difficult and where my time went throughout this exercise.

Thinking back now, I can honestly say that the majority of my time was spent grappling with Android's layout system and trying to get the RadialProgressView to work how I wanted it to.

I am actually a little bit familiar with the Android layout system, having produced a few applications back in the days of Android 1.0 and 1.5.  So I was able to get up and running with basic layouts for each of the pages that I was creating easily enough.

The problems arose with things like the RadialProgress extension, in that I didn't want a percentage to be the indicator in the middle of the circle.  This was solved easily enough by disabling that progress on the widget itself and overlaying my own text view with a MM:SS countdown as I'd wanted.

Towards the end of the project I thought that I'd simply add some background images to make each Activity's view a little more interesting to look at, and this was for the most part easy enough.  What was difficult was the Radial Progress widget is inherently transparent, and was very hard to read once you put a image background below it.  After a while, the solution presented itself, to simply draw a solid black circle behind the widget itself so that it would return to its normal, easily readable appearance.

It was things like these that became the real time sinks in the project.  Whilst there were certainly times where I was struggling to translate my knowledge of C# into something that could be used within F#, but this was rarely a blocking issue for too long.  F# itself is quite easy to pickup for people with a C# project, I found.

And when you run into trouble there is quite an abundance of resources on the web, be it StackOverflow or in the FSharp.org's various pages.

The Xamarin Android system itself wasn't hard to come up to speed with either.  Whilst all the documentation and examples I came across looking for the various solutions to the problems I was running into was in C#, it was simple enough to translate into the F# equivalent and be up and running in a couple of minutes.

It's interesting to think of the ways in which the newly released Android Watches can come into play with these sorts of applications.  Having a notification on your wrist when the eggs are boiled or ready to peel would be useful when cooking up a number of things at once in the kitchen.

All in all, this was a fun little project to sink some time into, and I've already got a couple of ideas for future projects that I could undertake with the Xamarin toolkit.
