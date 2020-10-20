a [g8] template for the most minimal Akka streams ML project
---

# UNDER CONSTRUCTION

# UNDER CONSTRUCTION

# UNDER CONSTRUCTION

A project generator for creating a working project that includes:
* an Akka Stream with a Kafka consumer source
* an Akka actor whose state is updated by the Akka stream
* an Akka HTTP REST API endpoint that inspects the Akka actor state via cURL or browser

## PREREQ

  * sbt >= 13.16

## USAGE

G8 will prompt you for details like your project name and package name

In a terminal shell, enter:

```console
sbt new navicore/actorflow.g8 
```

[g8]: http://www.foundweekends.org/giter8/

## CHALLENGE

* Modify the HTTP endpoint to accept a POST that updates the actor
* Create a second actor that accepts state change events from the first actor and publishes them to Kafka
* Make the actor "persistent" via event sourcing using https://doc.akka.io/docs/akka/current/persistence.html
* Enable the actor to inspect its earlier states via persistence journal queries

One possible solution to the above challenges is [here]()


## EXTRA CREDIT CHALLENGE

* Enable proper serialization in messaging and persistence
* Create a single cluster of multiple Akka Actor systems and enable actor sharding
* Enable multiple Akka Streams on multiple nodes consuming from a single Kafka topic
* Enable Kubernetes deployment as a statefulset
* Enable Kubernetes healthcheck and liveliness probe support
* Enable Kubernetes Prometheus monitoring leveraging the helthcheck endpoint above

One possible solution to the above extra extra challenges is [here]()
