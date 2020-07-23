# Distributed Caching

A cache stores data for quick access at a later time.

Caching is a technique to imporove performance and scalability

It will decrease response times and reduce load on downstream services and data sources.

The more static the data is, the longer it can be kept in a cache. You should use it for frequently requested data.

Types of caches:

* Private
    * In memory cache per JVM
* Shared
    * Shared caches across multiple service instances (Hazelcast)
* Internal
    * Cache is stored close to the consumer. In the same container.
* External
    * On an external service.
* Inline
    * Sits between the data source and the consumer. Consumer --- cache --- data source
    * Commonly used in web browsers
* Side
    * Sits separetly from the data source. cache --- consumer --- data source

What makes a cache distributed?

* Dynamic membership
* State coordination
* Members have a limited view

Common distributed caches:

* Infinispan
* Redis
* Terracotta EhCache
* Amazon Elasicache
* Memcache
* Hazelcast

Hazelcast:

In membory data grid (IMDG):

* Two topologies
    * Embeddeds
    * Client/server

Hazelcast Partitions:

* Single node cluster
* Dual node cluster

As you add more nodes to the cluster, you get more partitions and the shards will be shared accross them.

Hazelcast discovery mechanisms:

* TCP
* AWS Cloud
* Zookeeper
* Eureka
* Kubenetes
* Heroku

How is your cache kept up to date?

* Polling
    * Periodically checking source for updates
* Pushing
    * Source sends a message when there is an update
* Read-through updates
    * Get a request to read the cache and you find that the cache is out of date

