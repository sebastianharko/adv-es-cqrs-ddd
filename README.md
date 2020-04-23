# Advanced Topics in Event Sourcing / CQRS / DDD
Advanced Topics in Event Sourcing / CQRS / DDD. 

# Talks

* [Jonas Boner: How Events Are Reshaping Modern Systems (2017)](https://www.youtube.com/watch?v=3V3pHm2Cpks)
Event-driven architecture and design have been getting a lot of attention in recent years. It’s an old concept that has been around for decades, so why this sudden peak of interest?

* [Martin Krasser: Event Sourcing and CQRS with Akka Persistence and Eventuate (2015)](https://www.youtube.com/watch?v=vFVry457XLk)
Martin Krasser ([@mrt1nz](https://twitter.com/mrt1nz)), the original author of Akka Persistence and Eventuate, talks about CQRS, Event Sourcing with a focus on distributed systems and CAP tradeoffs. Spoiler: Akka Persistence is more on the CP side whereas Akka with Eventuate is more on the AP side. :star::star::star::star::star:

* [Data in Motion: Streaming Static Data Efficiently in Akka Persistence (2016) ](https://www.youtube.com/watch?v=K4FY0XKediU)
Martin Zapletal ([@zapletal_martin](https://twitter.com/zapletal_martin)) from Cake Solutions discusses details of Akka Persistence Query. From Akka docs: "Akka Persistence Query itself is not directly the query side of an application, however it can help to migrate data from the write side to the query side database."

* [Reification and type-safety in a CQRS world (2017) ](https://www.youtube.com/watch?v=qwYs0J7xp78) Renato Cavalcanti ([@renatocaval](https://twitter.com/renatocaval)) discusses how CQRS applications bring some new challenges for statically typed language lovers.

* [Event Sourcing & Functional Programming - a pair made in heaven (2015)](https://www.youtube.com/watch?v=1rFY2SfdDoE) Paweł Szulc ([@rabbitonweb](https://twitter.com/rabbitonweb)) talks about the relationship between FP and Event Sourcing. One of the implementations he shows makes use of the State monad and he briefly discusses how such an implementation works very well with property-based testing. 

* [The Elephant in the Room (2017)](https://skillsmatter.com/skillscasts/9652-the-elephant-in-the-room) by Greg Young. Discusses versioning.  

* [Building Apps with Functional Domain Models, Event Sourcing and Actors (2012)](https://www.youtube.com/watch?v=95KztoeGHl0) by Debasish Ghosh ([@debasishg](https://twitter.com/debasishg)). One of the most interesting parts is when Debasish points out a duality between event sourcing and functional data structures. 

* [Event in Software, Process, and Reality (2019)](https://www.youtube.com/watch?v=EX_zRTeowuM) by John Bywater. Discusses events as actual occasions of experience, and identifies the "process event" as the unit of reliability in systems of event sourced applications.

# Open Source

* [Stamina](https://github.com/scalapenos/stamina) Schema evolution for event sourcing. It has "*a strong focus on long-term viability of your persisted data so it provides support for versioning that data, auto-migrating that data at read time to be compatible with your current event and domain classes, and a testkit to make sure all older versions of your persisted data are still readable.*"

* [Event Sourcing for Akka Streams](https://github.com/krasserm/akka-stream-eventsourcing) by Martin Krasser ([@mrt1nz](https://twitter.com/mrt1nz)). Aims to provide a stateful EventSourcing graph stage for Akka Streams.

* [Fun.CQRS](https://github.com/strongtyped/fun-cqrs) An ES / CQRS framework with a pluggable backend (an Akka backend is provided). Even if you end up not using it, the code, in general, is a good illustration on how to create your own DSL and build your own abstraction over Akka's PersistentActor.

* [Akka Persistence Query Extensions](https://github.com/dnvriend/akka-persistence-query-extensions) "non-official akka-persistence-query-extensions contain components that are very handy to have for using akka-stream, akka persistence and akka query"

# Articles / Blog Posts

* [Hexagonal Architecture and Free Monad: Two related design patterns? (2017)](https://deque.blog/2017/07/06/hexagonal-architecture-a-less-declarative-free-monad/) by Quentin Duval.

* [Domain models, Algebraic laws and Unit tests (2017)](http://debasishg.blogspot.ca/2017/06/domain-models-algebraic-laws-and-unit.html) by Debasish Ghosh ([@debasishg](https://twitter.com/debasishg)).

* [Scalability using Sharding from Akka Cluster](http://michalplachta.com/2016/01/23/scalability-using-sharding-from-akka-cluster/) Michal Plachta ([@miciek](https://twitter.com/miciek?lang=en)) explains Akka Cluster Sharding. Note: he does not mention CQRS / ES / DDD but Cluster Sharding / Persistence are almost always used in combination. Cluster Sharding is useful even when you don't need high scalability since it provides passivation and manages actor creation for you (actor creation becomes "on demand").

* [Building a CQRS / ES Framework (part 1) (2017)](http://www.strongtyped.io/blog/2017/05/07/building-cqrs-es-framework-part1/) by Renato Cavalcanti ([@renatocaval](https://twitter.com/renatocaval)). Discusses the functional foundation of event sourcing. 

* [Akka Streams: A Motivating Example (2017)](http://blog.colinbreck.com/akka-streams-a-motivating-example/) You should read *everything* by Colin Breck ([@breckcs](https://twitter.com/breckcs?lang=en)) but this one in particular is a great start.

* [Akka Persistence: Testing Persistent Actors (2016)](http://tudorzgureanu.com/akka-persistence-testing-persistent-actors/) by Tudor Zgureanu ([@tudor_zgureanu](https://twitter.com/tudor_zgureanu)). Straight forward. Message in. Message out.

* [CQRS increases consistency (2016)](https://jazzy.id.au/2016/10/08/cqrs-increases-consistency.html) by James Roper ([@jroper](https://twitter.com/jroper?lang=en)). Fav quote: "*If someone says using CQRS in microservices means you lose consistency - they have failed to acknowledge that they lost consistency the moment they started using microservices, it was not CQRS that lost them that consistency.*"

* [Eventuate's documentation](http://rbmhtechnology.github.io/eventuate/) by Martin Krasser ([@mrt1nz](https://twitter.com/mrt1nz)) contains a wealth of knowledge and information and is an excellent read. :star::star::star::star::star:

# Academic Papers

* [The Dark Side of Event Sourcing: Managing Data Conversion (2017)](https://www.researchgate.net/publication/315637858_The_dark_side_of_event_sourcing_Managing_data_conversion) by Michiel Overeem, Marten Spoor, and Slinger Jansen ... Almost like the authoritative guide on versioning in event-sourced systems.

# More

PRs welcome. 

