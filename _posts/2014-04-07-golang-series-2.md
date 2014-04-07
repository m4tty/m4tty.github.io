---
layout: post
title: Measure All The Things (Day 2)
---

#Day 2 - Learning by doing

##Why is sending, storing, and using time-series data awesome?  Its all about feedback.

Before we start working on the time-series system, we'll go on a slight tangent to discuss why capturing metrics about your applications is important.

The speed at which we can receive feedback is a direct indicator of how quickly we can move through the software development cycle/workflow.  The shorter the feedback loop the quicker we'll be able to react, and the quicker (and more) we'll be able to push change and innovate.  We want to transform our organizations into fast moving and high performing environments... and in order to do so we must create an software factory that shortens the cycles to push change and receive feedback in order to gain a competitive advantage.  Without short feedback loops we are rate limiting our ability to change.

**What should be measured?**  Everything.

###Application, System, Network measurements.

####Application Metrics
Any function that provides value or insight into an application should be timed or counted and sent.

####System
Understanding the health of your servers is of paramount importance.  The standard set of information to capture is Memory, CPU, and disk.  See [CollectD](http://collectd.org/).

####Network
Having visibility into the health of the network is also important when troubleshooting.  To begin with, using tools that live with the System/Machine to get a view into the network health (as the machine perceives its own network interface) is a good start.  Ultimately, using correlation identifiers to act as tracer "bullets" that can capture points in time as requests move throughout our networked systems.  See [Zipkin](http://twitter.github.io/zipkin/), [Dapper](http://static.googleusercontent.com/media/research.google.com/en/us/pubs/archive/36356.pdf), [CollectD](http://collectd.org/), [Ping Script](http://obfuscurity.com/2012/07/El-Cheapo-Network-Graph)

####Error counts
Another valuable data point is your Error logs.  Error logs can be parsed and counted, making it possible to monitor for fluctuations in Error rates and trend on specific Error strings.  You can send these to Graphite, but this is also a great place to use [Logstash](http://logstash.net/), [Elastic Search](http://www.elasticsearch.org/), and [Kibana](http://www.elasticsearch.org/overview/kibana/).

####Capture Change Events (track every release)
Changes to our application code are opportunities for the introduction of issues.  By tracking change events (deploys) we can correlate metric fluctuations to causation from the change event.  Application Metrics + Change Events are keys to providing confidence and enabling change (i.e Continuous Deployments).


####Amplify the feedback
Display a wallboard for goodness sakes.  Use a large display that shows always relevant, easy to understand, graphs.  Atlassian explains it well [here](http://www.slideshare.net/GoAtlassian/ltds3-information-radiators) and [here](https://blogs.atlassian.com/2011/10/using_an_appletv_as_a_build_monitor/).

![Wallboard](/public/images/kCeDD.jpg)


###Monitoring (Application, System, Network metrics)
####Use the Humans: 
Amplify the feedback (graphs) by using a wallboard.  Humans watch the graphs for fluctuations during deploys and are happy.
 
####Use the Machines:
In order to use the machines for monitoring we must talk about normal trends.  What is abnormal?  For monitoring, it is important to look at normal and abnormal. Most monitoring is done with static thresholds for alarms and alerts, but in our applications thresholds change over time and at different times of the day.  Our systems might see a huge variance in response, but we would likely receive no alerts if we have set a high static warning threshold.  Large spikes during business peaks can be normal and the troughs can be just as extreme during lows, so thresholds need to be dynamic.  One way we can better monitor and alert is using something like the Holt-Winters exponential smoothing algorithm for predicting confidences (upper and lower bounds) and plotting aberrations.


###Summary
Whether you use Graphite, what we -eventually- build, or something else entirely, you should definitely be capturing and monitoring your application and system metric data.  Now that you know why it is important, I hope you'll be -at least a bit more- excited to build a time-series system.

Next, we'll do a little bit of architecture/design.



