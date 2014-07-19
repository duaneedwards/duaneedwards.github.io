---
layout: post
published: true
title: "Monkey Business #2"
quote: Xamarin Android and F# Gotchas
image: "/media/MonkeyBusiness2cover.jpg"
video: false
---
## Xamarin Android and F# Gotchas

Being completely new to F#, and coming from a strong C# background, one thing that threw me for a loop for a little while was the way in which you reference other code in F#.

For a while the only way that I could get the project to build with all five activities was to simply put all of the activities in the main code file.

After I had made a little progress into the project I decided to revisit this and find the cause of why I couldn't have separated out my various activities and have the solution compile.  What I found was that the build order of the files is important in FSharp, and that you need to order the files in your solution in the order that you'd like them to be built in.

Not only that, but it seems that you can't reference code that hasn't been built yet in the solution.  Which is quite a change if you come from another programming language background and are used to having the compiler handle such linking operations automagically.

However once I figured out what the problem was, it was simple enough to extract out the various activities into their own code files and have the solution compiling as I wanted it to.

One thing that caught me out on multiple occasions was the difference in the usage of the assignment operator in F#.

```
progress.Value = 0.5f // C# assignment
```

```
progress.Value <- 0.5f // F# assignment
```

I stumbled upon this link which broke down the differences quite well and is a recommended read if you are new to F#:

[Assignment operator in F#](http://stackoverflow.com/questions/5534368/assignment-operator-in-f)

Other than that the differences I've come across are merely syntactical, i.e things like this.

```
typeof(SomeClass) // C#
typeof<SomeClass> // F#

Action something -> { doStuff() } // C#
fun _ -> doStuff(); // F#
```

Despite not knowing the language, I've been making reasonable progress in a short time.  Not to mention in a new development environment on a new platform to me :-)
