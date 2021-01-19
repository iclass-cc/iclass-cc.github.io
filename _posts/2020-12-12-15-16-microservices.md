---
key: 2020-12-12-15-16-microservices
title: Microservices 微服务架构
date: 2020-12-12 15:16 +0800
tags: Computer Science 计算机科学
---

![Microservices](https://tenetai.com/iclass/m.png)

Microservice architecture – a variant of the service-oriented architecture (SOA) structural style – arranges an application as a collection of loosely coupled services. In a microservices architecture, services are fine-grained and the protocols are lightweight.

A consensus view has evolved over time in the industry. Some of the defining characteristics that are frequently cited include:

- Services in a microservice architecture (MSA) are often processes that communicate over a network to fulfil a goal using technology-agnostic protocols such as HTTP.
- Services are organized around business capabilities.
- Services can be implemented using different programming languages, databases, hardware and software environment, depending on what fits best.
- Services are small in size, messaging-enabled, bounded by contexts, autonomously developed, independently deployable, decentralized and built and released with automated processes.

A microservice is not a layer within a monolithic application (example, the web controller, or the backend-for-frontend). Rather it is a self-contained piece of business functionality with clear interfaces, and may, through its own internal components, implement a layered architecture. From a strategy perspective, microservices architecture essentially follows the Unix philosophy of "Do one thing and do it well".

Martin Fowler describes a microservices-based architecture as having the following properties:

- Lends itself to a continuous delivery software development process. A change to a small part of the application only requires rebuilding and redeploying only one or a small number of services.
- Adheres to principles such as fine-grained interfaces (to independently deployable services), business-driven development (e.g. domain-driven design).

It is common for microservices architectures to be adopted for cloud-native applications, serverless computing, and applications using lightweight container deployment. According to Fowler, because of the large number (when compared to monolithic application implementations) of services, decentralized continuous delivery and DevOps with holistic service monitoring are necessary to effectively develop, maintain, and operate such applications.

A consequence of (and rationale for) following this approach is that the individual microservices can be individually scaled. In the monolithic approach, an application supporting three functions would have to be scaled in its entirety even if only one of these functions had a resource constraint. With microservices, only the microservice supporting the function with resource constraints needs to be scaled out, thus providing resource and cost optimization benefits.

<!--more-->
