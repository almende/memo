---
layout: default
title: Introduction
---

# Introduction

Memo provides shared and distributed memory data structures and tools. One of these 
tools are multi-agent systems that are especially equipped for building decentralized
systems. 

Our data structures and tools can be divided into several categories: 
- [Distributed data models](#databases)
- [Gossiping](#gossiping)
- [Caching mechanisms](#caching)

## Distributed data models {#databases}

Memo aims not to support just one distributed database, but aims to benefit from different
ones depending on the task at hand. We aim to support:

- [Hadoop](http://hadoop.apache.org/) a free implementation of [MapReduce](http://en.wikipedia.org/wiki/MapReduce)
- [GraphLab](http://graphlab.org/) a distributed machine learning (belief propagation) in the cloud
- [Akka](http://akka.io/) an actor toolkit 
- [Eve](http://almende.github.com/eve/) our own actor toolkit

## Gossiping {#gossiping}

Although memo does not provide many algorithms for all kind of machine learning tasks (see
for that the [Nets](http://almende.github.com/nets) module in the CHAP toolbox), it does
provide a few algorithms that are intertwined with the nature of data storage. One of the
mechanisms we provide is so-called [gossiping](http://en.wikipedia.org/wiki/Gossip_protocol).

Gossiping is used to communicate data in the wireless sensor networks of one of our daughter
companies: [Sense](http://www.sense-os.nl/)

## Caching {#caching}

Memo provides means to cope with non-functional behaviour that comes with data storage and
handling. Caching is just one facet of a solution with respect to the user experience. To be 
able to cope with latency, multiple copies of data can be stored across the networks, etc.
Tradeoffs need to be made between [location transparency](http://en.wikipedia.org/wiki/Location_transparency) 
(the ability to run whereever you are) versus [location awareness](http://en.wikipedia.org/wiki/Location_awareness)
(the ability to take into account your environment).

## Open source {#opensource}

Our algorithms are offered as open-source software under LGPLv3 or Apache license. Almende 
and spin-offs use it in their commercial products, which contribute to their maturity.
