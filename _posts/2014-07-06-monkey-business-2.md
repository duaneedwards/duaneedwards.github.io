---
layout: post
published: false
title: "Monkey Business #2"
quote: Xamarin Android and F# Gotchas
image: "/media/MonkeyBusiness2cover.jpg"
video: false
---
## Xamarin Android and F# Gotchas

C#:
typeof(SomeClass)

F#:
typeof<SomeClass>

Referencing other classes in F# is a bit interesting ...
For now I'll just bung them all in the same class.

Assigning variables:
C#:
progress.Value = 0.5f

F#:
progress.Value <- 0.5f

[Helpful Link](http://stackoverflow.com/questions/5534368/assignment-operator-in-f)

Separate Activities timer's elapsed events being invoked Across activity types?!
