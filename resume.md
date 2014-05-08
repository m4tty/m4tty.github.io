---
layout: page
title: Resume
---

##Matthew Self

#### 2158 Fox Fire St, Highlands Ranch, CO • self.matt@gmail.com

* [LinkedIn](http://www.linkedin.com/pub/matt-self/1/961/503)
* [StackOverflow](http://stackoverflow.com/users/1442914/matt-self)


---
<div class="message">
  Software Engineer and Architect with over 15 years experience building large scale software intensive systems using a wide variety of languages and technologies.
</div>

---

##Experience

##Chief Architect - Pearson - (1999 - Present)

### Student Event Feed
Designed and implemented a near real-time, fault tolerant, user event stream leveraging Node.js and MongoDB. System allowed for the efficient construction of web pages and REST endpoints for showing latest events in a student’s activity feed. Due to the high fanout nature of the event sources (i.e. many disparate domains publishing events), system achieved excellent performance and efficiency by selectively materializing each user’s feed. Workloads with a high query rate were materialized at event time, while user’s with a low query rate were materialized on-demand at query time.

* Architecture resulted in a low cost per transaction and high scalability at just over 200 requests per second on small cloud instances.
* Processed and stored over 150 million messages with 100% success for process-able messages and have successfully handled all bad/dead messages with no failures.
* Easily exceeded 1000 requests per second with no success rate degradation or increased latency.

### Event Enrichment System
Created a scalable and fault tolerant system for enriching messages beyond what the source system could provide by collaborating asynchronously with other data providers. This allowed internal system messages to remain simple, while the event enricher added information to meet the external party contract. Leveraged Node.js to handle I/O bound data enrichment workload and so were able to handle hundreds of thousands of events concurrently.

### Cloud Latency, Variability, and SOA Analysis Team
Led effort to operationalize cloud computing against the backdrop of a Service Oriented Architecture. Performed a measurement study to understand latency and latency variability impact in a large system of networked dependencies on virtualized cloud resources. Recommendations resulted in modifications to planned cloud deployment topology and reduced latency and latency variability.

### Student Gamification System
Designed and implemented extensible Gamification system to increase student engagement. System was created to allow for the experimentation and reconfiguration of new challenges through the use of A/B testing and measurement to ensure effectiveness in driving desired behavior and to prevent the dilution of rewards.

### Collaborative Student Groups
Designed and implemented real-time collaborative student essay system leveraging Node.js and socket.io and backed by Java and Cassandra. Successfully deployed and leveraged Cassandra in a multi-region cloud environment which contributed to low latency data retrieval for clients in both East and West regions.

### “Web Services on Demand” Platform
Created composable REST APIs for over 20 business domains. This effort spearheaded a major shift toward a Service Oriented Architecture and positioned the organization and the software ecosystem to be more resilient and flexible to both technical and business changes.

### OpenClass Learning Management System
Architect and engineer for a team building the student and professor dashboard for the then next generation LMS. By leveraging the latest web best practices the team was able to significantly reduce web page load time.

### Course "Home" Page Performance Tuning and Analysis
Performed analysis and corresponding corrections which resulted in reducing page load times by over 5 seconds through the reduction of HTTP requests, prefetching, page reorganization, non-blocking script loading, CDN resource and AJAX caching.

### "Measure Everything" initiative
Amplified and introduced the usage of instrumentation metrics and monitoring as a means to shorten software feedback loop.  Incorporated the usage of StatsD and Graphite for measuring application, machine, and network metrics throughout the software ecosystem.  Introduced software change events and anomaly detection in order to increase confidence in continuous delivery process and speed the rate of innovation.

### Hackathons and Wallboards
Championed and helped introduce and run Hackathons as a means to drive disruptive innovation.  Hackathons helped facilitate a culture of learning and making outside of the well worn grooves of daily development.  Won two hackathons, one of which was eventually grown into the student Gamification product.
Spread the usage of Wallboards to display critical team application information by introducing and evangelizing the first Wallboard as a team information radiator.  This practice was copied by teams throughout the organization and increased confidence, ownership, and ultimately resulted in reducing mean time to issue discovery across the organization and helped increase the frequency of releases. 

### .NEXT Continuous Delivery
Evangelized continuous delivery practices in the legacy .NET application stack in the form of explicit dependencies, static packages, build, package, and deploy automation, and separating release and deploy, in order to increase the rate of change. Introduced tools that incentivized continuous delivery in the .NET development lifecycle to allow for shorter feedback cycles, shared ownership, system decomposition, risk isolation, and increased agility.


### .NEXT Learning Management System

Engineer and architect on “enterprise” infrastructure for the primary learning platform. Scaled .NET applications to thousands of requests per second and over seventy five million user minutes per day. Introduced strong domain, scale, and fault boundaries in order to support business and technology flexibility. By predicting areas of anticipated variation and creating boundaries around them, we were able to scale and grow systems in isolation.

---

##Technical Skills

**Languages:** javascript, node.js, Java, C++, C#, Go, python, ruby, HTML, CSS

**Storage:** Cassandra, MongoDB, Redis, SQL Server, MySQL

**Technologies / Frameworks:** bootstrap.js, angular.js, jquery, graphite, puppet, fabric, RabbitMQ, ASP.Net, HAProxy, Nginx, IIS

**Platforms:** Unix/Linux, Windows

**Cloud Providers:** Amazon AWS, Google Compute Engine

**Tools and Methodologies** SOA, REST, HTTP, OOA/D, SOLID, Agile, TDD, UML, Design Patterns


---
##Education
University of Florida - Bachelors of Science, 1999


