---
layout: post
title: "The 'soft' Skills in Testing"
date: 2015-04-22 11:55:00
cover: cucumber_stockphoto.jpg
categories: posts
---

##Writing Cucumber Scenarios - Why we should leave the code out.

I currently find it hard to swap between the needs of being a coder and a tester*. Being inexperienced I am still required to wear both hats at the same time like some experienced developers do.  What this has been doing though, is affecting the way I write cucumber scenarios with fellow colleagues.

Automatically I find myself implementing the DRY (Don’t Repeat Yourself) principle.  In learning to structure my code and reduce the chances of my mistakes being harder to find (at my current stage there is enough of them!), I like to make sure that my code is not repeated in several places.  

Following this principle as a tester can prove to be a double edged sword.  With scenarios, I found myself creating lines such as `"Given I log in"` which would be used repeatedly for that very action.

Don't get me wrong, there is an element of reusability with actions such as this, but the more we do it the more we feel the need to reuse scenario lines even when it might not be suitable.  

Scenarios are used to describe the actions of a user travelling through our system, when they do something as well as what they expect to happen.  When using the DRY principle you can lose sight of the subtlety of peoples behaviour.  Cucumber scenarios are clean and easy to read, however while they are written using the Gherkin syntax, they are also written in English to improve accessibility.  

We should use this to paint the journey that our user takes us on and use it to make it interesting to read; its the living documentation of our system! People should want to read it!

My current aim is to shove the DRY principles back where they belong; with the code.  Using DRY means that you can drive step definition code into methods and reduce the real repetition.

Cucumber scenarios were developed to allow the tech to talk to the business, and allow the tech to understand the behaviour of the system that they are developing.  Working together to achieve this single goal requires a cohesive language which can be marred by perceived efficiencies.

So yeah, in dropping the DRY principle from my scenarios I can use language to paint clearer user behaviour in a system!

*I say 'coder' instead of developer as I class both coder and testers as types of developers, but I differentiate them here as I feel they carry two different mindsets.
