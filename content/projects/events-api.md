+++
author = "Ramona E.J. Spence"
title = "Events API"
date = "2022-02-14"
description = "Open Source project organized by Code for Greenville"
tags = [
    "api", "project",
]
summary = "Finding tech-related meetups that are in your area can be a bit of a pain when they're often split among platforms. Code for Greenville aims to solve that problem for the Upstate of South Carolina by bringing these events to one place"
+++

[*Check out this project on Github!*](https://github.com/codeforgreenville/upstate_tech_cal_service)

Finding tech-related meetups that are in your area can be a bit of a pain when they're often split among platforms. Code for Greenville aims to solve that problem for the Upstate of South Carolina by bringing these events to one place.

## **What is it?**
First off, an API is an **A**pplication **P**rogramming **I**nterface. In essence, an API is the interface between two applications that allows them to share data and communicate.

The Events API provides data on events related to the tech and software industries in JSON format, but first, there's an application that gathers that data and formats it. I get to work on these two parts!

Now, other applications can query the API, receive the data, and use it in various ways. [HackGreenville.com](https://hackgeenville.com), for example, consumes the API to fill its calendar with tech-related events!

## Javascript Object Notation

I mentioned that the Events API uses a JSON format. This stands for **J**ava**S**cript **O**bject **N**otation. 

JSON is a data-interchange format. It's completely language independent, and therefore data in JSON format is interchangeable between applications, no matter what langauges those applications use.

So the Events API is essentially an application that gathers data on tech-related events in a format that can be easily understood by both humans and applications, and then serves that data in a way that it can be accessed by other applications.


## Linked Data and Context

This is all awesome, but there are still ways for this API to be even more useful. 

We've recently added support for JSON-LD. The "LD" on the end stands for **L**inked **D**ata. This format uses a _context_ that allows search engines to understand and use the data that's there. In this case, the context used is [Schema.org](https://schema.org/).

To explain this, let's say we have a field called `start_date`. You and I can probably infer what the name means, but a search engine will only see a string of characters with a datetime object attached to it. 

With a context like Schema, we have things like an [Event](https://schema.org/Event) which has properties already defined. And `startDate` is one of them!

Now, a search engine can understand and do something with that information. Pretty cool, right?