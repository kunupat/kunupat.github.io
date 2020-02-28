---
title:  "How To Run Go Executable And Java In Single Docker Container"
date:   2020-02-28
---

How to run two processes in a Docker container. In this example, I run a GoLang REST Server and SpringBoot REST Client in single Docker container.

## Is it right?
As [per this document][1], it appears that it's an anti-pattern to run multiple services in one Docker container. But after re-reading the document, my understanding is that we should have one _service_ per container. This services can spawn multiple _processes_ like Apache web server starts multiple worker processes. So I think it's ok to have multiple processes in a Docker container in case our use case really really needs it.

E.g. This kind of architecutre may be good for running a batch application that depends on a REST API and cannot afford to make REST calls over the network. 

## Sample Apps

### Simple REST Server Written In GoLang
[Github Repo][2]


### Simple REST SpringBoot Client
[Github Repo][3]

[1]: https://docs.docker.com/config/containers/multi-service_container/
[2]: https://github.com/kunupat/GoRestServer/tree/master
[3]: https://github.com/kunupat/SpringRestClient
