---
layout: page
title: Resume
---

##Matthew Self

#### 2158 Fox Fire St, Highlands Ranch, CO • 720.231.2305 • self.matt@gmail.com

* [LinkedIn](http://www.linkedin.com/pub/matt-self/1/961/503)
* [StackOverflow](http://careers.stackoverflow.com/cv/edit/176752)


---
<div class="message">
  Software Engineer and Architect with over 15 years experience building large scale software intensive systems using a wide variety of languages and technologies.
</div>

---
##Chief Architect - Pearson - (1999 - Present)

<div class="message">
  Software Architect responsible for implementing highly scalable web-based software solutions targeting the learning domain.
</div>


---
##Experience

### Cloud Latency and Variability Analysis
Led effort to operationalize cloud computing against the backdrop of a Service Oriented Architecture.  Performed a measurement study to understand latency and latency variability impact in a large system of networked dependencies.  Analysis resulted in modifications to planned cloud deployment topology.

* Created transparent private load balancers to handle service discovery in the cloud.
* Led the creation of a framework to automate service registration and discovery.

### User Event Feed
Designed and implemented a near real-time, fault tolerant, user event stream using Node.js and MongoDB.  System allowed for the efficient construction of web pages and REST endpoint for showing latest events in a user’s feed.  Due to the high fanout nature of the event sources (i.e. many disparate domains publishing events), system achieved best performance and efficiency by selectively materializing each user’s feed.  Workloads with a high query rate are materialized at event time, while user’s with a low query rate are materialized on-demand.

* Architecture resulted in an extremely low cost per transaction and high scalability.
* Processed and stored over 70 million messages with 100% success for process-able messages and have successfully handled all bad/dead messages with no failures.
* Easily exceeded 1000 requests per second with no success rate degradation or increased latency.

### Event Enricher
Created a scalable and fault tolerant system for enriching messages beyond what the source system could provide by collaborating asynchronously with other data sources.  This allowed internal system messages to remain simple, while the content enricher added information to meet the external party contract.  Leveraged Node.js to handle I/O bound data enrichment workload and so were able to handle hundreds of thousands events concurrently. 

### Student Gamification System
Designed and implemented extensible Gamification system to increase student engagement.  System events are judged against configurable criteria to determine rewards. 

### Collaborative Student Groups
Designed and implemented real-time collaborative student essay system backed by Java and Cassandra.

### “Web Services on Demand” Platform
Created composable REST APIs for over 20 business domains.  This effort pushed a major shift toward a Service Oriented Architecture and positioning the organization and the system to be more resilient and flexible to both software and business change.

### OpenClass Learning Management System
Architect and engineer for team building the student and professor dashboard for next generation LMS.

### Client Side Performance Tuning and Analysis 
Analysis and corresponding corrections resulted in reducing page load times by over 5 seconds by reducing HTTP requests, prefetching, page reorganization, non-blocking script loading, CDN resource and AJAX caching.

### Measure Everything
Amplified and introduced the usage of instrumentation metrics and monitoring as a means to shorten software feedback loop.  Incorporated the usage of StatsD and Graphite for measuring application, machine, and network metrics throughout the software ecosystem.  Introduced software change events and anomaly detection in order to increase confidence in continuous delivery process and speed the rate of innovation.

### Culture Change
Championed and helped introduce and run Hackathons as a means to drive disruptive innovation and facilitate a culture of learning and making outside of the well worn grooves of daily development.  
Spread the usage of Wallboards to display critical team application information which increased confidence and ultimately resulted in reducing mean time to issue discovery across the organization and helped increase the frequency of releases.  Introduced the first Wallboard as a team information radiator, this led to hundreds of Wallboards throughout the organization and had a far reaching impact

### Continuous Delivery
Evangelized continuous delivery practices in the legacy .NET application stack in the form of explicit dependencies, static packages, automation, and separating release and deploy, in order to increase the rate of change.  Introduced tools that incentivized continuous delivery in the .NET development lifecycle to allow for shorter feedback cycles, shared ownership, system decomposition, risk isolation, and increased agility. 

### .NEXT Learning Management System

Engineer and architect on “enterprise” infrastructure for the primary learning platform.  Scaled .NET applications to thousands of requests per second and over seventy five million user minutes per day.  Introduced strong domain, scale, and fault boundaries in order to support business and technology flexibility.  By predicting areas of anticipated variation and creating boundaries around them, we were able to scale and grow systems in isolation.

---

##Technical Skills

**Languages:** javascript, node.js, Java, C++, C#, Go, python, ruby, HTML 5

**Storage:** Cassandra, MongoDB, Redis, SQL Server, MySQL

**Technologies / Frameworks:** ASP.Net, bootstrap.js, angular.js, jquery, graphite, puppet, fabric

**Applications / Web Servers:** HAProxy, Nginx, IIS

**Platforms:** Unix/Linux, Windows

**Cloud Providers:** Amazon AWS, Google Compute Engine

**Tools and Methodologies** OOA/D, SOA, REST, SOLID, Agile, TDD

---
##Education
University of Florida - Bachelors of Science, 1999

---
##References
Available upon request.

