# Microservices - The Practical Way - v8

This project contains the version 8 of the application that is developed under the scope of the book Microservices - The Practical Way. 
You can get a copy of the book on [Leanpub](https://leanpub.com/microservices-thepracticalway).

## Contents

The repository contains five folders, one for each component of the system:

* **social-multiplication** is one of the backend services. It has a REST API to get and provide results to simple multiplications. When an attempt is sent, it triggers an *event*.
* **gamification** is the second backend service. It provides a REST API to get game stats and reacts to the event sent by the multiplication service, updating the figures.
* **service-registry** is the Eureka Server, which is contacted by backend services and the gateway.
* **gateway** is the Routing Service, implemented with Zuul. It connects with Eureka for service discovery, and performs load balancing with Ribbon.

