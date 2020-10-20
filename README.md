a [g8] template for the most minimal Akka streams ML project
---

A project generator for creating a working project that includes:
* a Kafka consumer
* an Actor system
* an Actor whose state is updated by Kafka traffic
* a REST that inspects the actor state

## PREREQ

  * sbt >= 13.16

## USAGE

G8 will prompt you for details like your project name and package name

In a terminal shell, enter:

```console
sbt new navicore/navistream.g8 
```

[g8]: http://www.foundweekends.org/giter8/

## EXTRA CREDIT CHALLENGE

* see if you can add a POST route to the REST API that updates the actor
* see if you can create an new actor that accepts data from the example actor and publishes that data to Kafka
