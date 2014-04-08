---
layout: post
title: Learning Go by Building a Time-Series System (Intro - Day 1)
---

#Day 1 - Learning by doing

##Let’s build something in Go together

I’ve been programming Go for a little while now, and have been plugging along, but I haven’t built anything truly useful or challenging.  So, in an effort to [“learn by doing”](http://en.wikipedia.org/wiki/Experiential_learning), I’ll be attempting to build something non-trivial and along the way I’ll share all of the gory details from soup to nuts.

Instead of building yet another blog engine or a to-do list application I’ve decided to build a time-series data store, services, and graphing engine.  Much of what we build will be similar to functionality in -the oh so awesome- [Graphite](http://graphite.wikidot.com/) (and [statsd](https://github.com/etsy/statsd/)).  While I don’t think we’ll build *all* of the parts required, we will attempt to write the software ourselves in places where learning opportunity and low difficulty intersect.  We’ll leverage and collaborate with open source software when the task is too great or doesn’t contribute to learning Go.

The high level plan will look like this: 

- We'll start with some context (i.e. why measure all the things) about why a time-series system is cool to build.
- Then we'll do some design and architecture.
- Set up our programming environment and level set on Go.
- Start coding...

<div class="message">
Along the way I'll take a number of tangents, where it is something I think is worth learning or explaining.  When I do so, I'll try to designate those sections differently.
</div>

###The High Level Functional Requirements

**Store numeric time series data**

- UDP for high frequency, finely grained data points, and clients that need to fire and forget
- HTTP for aggregated data
- Low storage footprint
- High precision for more recent data, lower precision as data ages

**Retrieve numeric time series data**

- HTTP
- Server side data functions support

**Graphs**

- Simple, good looking, plotted graphs
- Doesn’t need to be interactive

###Additionally, we want:

- Testable software
- Decent test coverage
- Documentation
- Fun (if it isn’t fun to build it, we won’t)
- Learning (we’ll take some detours along the way when appropriate)
- A design/architecture that supports change in key areas

##Following along at home

I’ll be using git / github to manage the changes over time.  I’ll be providing commit ids along the way for the folks that would like to follow along.


##Summary

I'm going to build a time-series system and while I do so I will write down all of the ugly details along the way.  You can follow along and we'll learn something together.


