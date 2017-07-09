# Advanced Topics in Event Sourcing / CQRS / DDD
Advanced Topics in Event Sourcing / CQRS / DDD

# Talks

* [Martin Krasser: Event Sourcing and CQRS with Akka Persistence and Eventuate (2015)](https://www.youtube.com/watch?v=vFVry457XLk)
Martin Krasser, the original author of Akka Persistence and Eventuate, talks about CQRS, Event Sourcing with a focus on distributed systems and CAP tradeoffs. Spoiler: Akka Persistence is more on the CP side whereas Akka with Eventuate is more on the AP side.
* [Sane Sharding with Akka Cluster (2016)](https://www.youtube.com/watch?v=f06Otw_DuQU) Michal Plachta explains Akka Cluster Sharding. Note: he does not mention CQRS / ES / DDD but Cluster Sharding / Persistence are almost always used in combination. Cluster Sharding is useful even when you don't need high scalability since it provides passivation and manages actor creation for you (actor creation becomes "on demand").
* [Data in Motion: Streaming Static Data Efficiently in Akka Persistence (2016) ](https://www.youtube.com/watch?v=K4FY0XKediU)
Martin Zapletal from Cake Solutions discusses details of Akka Persistence Query. From Akka docs: "Akka Persistence Query itself is not directly the query side of an application, however it can help to migrate data from the write side to the query side database."
* [Reification and type-safety in a CQRS world (2017) ](https://www.youtube.com/watch?v=qwYs0J7xp78) Renato Cavalcanti discusses how CQRS applications bring some new challenges for statically typed language lovers.
* [Event Sourcing & Functional Programming - a pair made in heaven (2015)](https://www.youtube.com/watch?v=1rFY2SfdDoE) Paweł Szulc talks about the relationship between FP and Event Sourcing. One of the implementations he shows makes use of the State monad and he briefly discusses how such an implementation works very well with property-based testing. 
* [Functional API for defining type safe, reliable Akka actors (2016)](https://www.youtube.com/watch?v=GsPAHzk8-mE) By Daniel Urban.
* [Building Apps with Functional Domain Models, Event Sourcing and Actors (2012)](https://www.youtube.com/watch?v=95KztoeGHl0) By Debasish Ghosh. One of the most interesting parts is when Debasish points out a duality between event sourcing and functional data structures. 

# Open Source
* [Stamina](https://github.com/scalapenos/stamina) Schema evolution for event sourcing.
* [Event Sourcing for Akka Streams](https://github.com/krasserm/akka-stream-eventsourcing) by Martin Krasser. Aims to provide a stateful EventSourcing graph stage for Akka Streams.
* [Fun.CQRS](https://github.com/strongtyped/fun-cqrs) An ES / CQRS framework with a pluggable backend (an Akka backend is provided). Even if you do not end up using it, the code, in general, is a good illustration on how to create your own DSL and build your own abstraction over Akka's PersistentActor.

# Articles / Blog Posts
* [Hexagonal Architecture and Free Monad: Two related design patterns? (2017)](https://deque.blog/2017/07/06/hexagonal-architecture-a-less-declarative-free-monad/) by Quentin Duval.
* [Domain models, Algebraic laws and Unit tests (2017)](http://debasishg.blogspot.ca/2017/06/domain-models-algebraic-laws-and-unit.html) by Debasish Ghosh.
* [Building a CQRS / ES Framework (part 1) (2017)](http://www.strongtyped.io/blog/2017/05/07/building-cqrs-es-framework-part1/) by Renato Cavalcanti. Discusses the functional foundation of event sourcing. 
* [Akka Streams: A Motivating Example (2017)](http://blog.colinbreck.com/akka-streams-a-motivating-example/) You should read *everything* by Colin Breck but this one in particular is a great start.
* [Akka Persistence: Testing Persistent Actors (2016)](http://tudorzgureanu.com/akka-persistence-testing-persistent-actors/) 

# Academic Papers
* [The Dark Side of Event Sourcing: Managing Data Conversion (2017)](http://files.movereem.nl/2017saner-eventsourcing.pdf) by Michiel Overeem, Marten Spoor, and Slinger Jansen ... Almost like the authoritative guide on versioning in event-sourced systems.
