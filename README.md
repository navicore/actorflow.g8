a [g8] template for a working digital twin starter project consisting of an Akka Stream and Akka Actors
---

# UNDER CONSTRUCTION

# UNDER CONSTRUCTION

# UNDER CONSTRUCTION

A project generator for creating a working project that includes:
* an [Akka Stream] consuming from [Kafka]
* a system of [persistent] [Akka actors] whose state is updated by the [Akka stream]
* an [Akka HTTP] REST API endpoint that inspects the [Akka actor] state via [cURL] or browser
* a [Kafka] producer that writes state change events to [Kafka]

## PREREQUISITE

  * sbt >= 13.16

## BUILDING

G8 will prompt you for details like your project name and package name

In a terminal shell, enter:

```console
sbt new navicore/actorflow.g8 
```

## DESKTOP DEVELOPER USAGE

Prerequisite: [Docker]

### Init Kafka

#### TBD

### Init Postgres

#### TBD

## DESKTOP KUBERNETES DEPLOYMENT

### TBD

## CLOUD KUBERNETES DEPLOYMENT

### TBD

## CHALLENGE

### TBD

## CHALLENGE

### TBD

One possible solution to the above challenges is [here]()


## EXTRA CREDIT CHALLENGE

# TBD

One possible solution to the above extra extra challenges is [here]()

[persistent]: https://doc.akka.io/docs/akka/current/persistence.html
[g8]: http://www.foundweekends.org/giter8
[Akka stream]: https://doc.akka.io/docs/akka/current/stream/index.html
[Akka HTTP]: https://doc.akka.io/docs/akka-http/current/index.html
[Kafka]: https://kafka.apache.org
[Akka actors]: https://doc.akka.io/docs/akka/current/actors.html
[Akka actor]: https://doc.akka.io/docs/akka/current/actors.html
[cURL]: https://curl.haxx.se/
[Docker]: https://www.docker.com/products/docker-desktop
