---
title: "Golong Distributed Cache"
excerpt: "

A lightweight, in-memory distributed caching system implemented in Go, designed for scalability and simplicity.
This project is a distributed in-memory key-value cache built in Go, designed to demonstrate core principles of scalable system design. It uses gRPC for communication between cache nodes and supports basic operations like Get, Set, and Delete. Keys are distributed across nodes using consistent hashing, which ensures load balancing and minimizes data movement when nodes are added or removed.

Each node includes an LRU-based local cache and acts as both a server and client, forwarding requests to the correct node if needed. An HTTP gateway provides a simple REST API interface for users, internally routing requests via gRPC.

The system is modular and can be extended with features like persistence or replication. This project is ideal for understanding distributed coordination, request routing, and cache eviction strategies using Go and gRPC. It includes unit tests and documentation to help developers quickly run and experiment with a multi-node setup.  [Github repository](https://github.com/sherryyiyang/go-distributed-cache)


<br/><img src='/images/distributed-cache.svg'>"
collection: "https://github.com/sherryyiyang/go-distributed-cache"

---

[https://github.com/sherryyiyang/go-distributed-cache](https://github.com/sherryyiyang/go-distributed-cache)

This repository contains my Go implementations of distributed systems primitives from MIT 6.5840: Distributed Systems. Projects include a simplified MapReduce framework with task scheduling, worker registration, fault tolerance, and coordination between mappers and reducers for parallel data processing; a full Raft consensus algorithm implementation covering leader election, log replication, term persistence, and crash recovery; a replicated key/value store layered on Raft that guarantees linearizability under failures; a sharded key/value service that supports dynamic configuration and shard migration between replica groups; and a persistent key/value store with snapshotting and state recovery to handle large logs and node restarts. Each module is built with a focus on fault tolerance, concurrency, and distributed correctness under real-world conditions.