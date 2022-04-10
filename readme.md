# Twelve Factor Application
Based on [This](https://12factor.net/) documentation

## Introduction
In the modern era, software is commonly delivered as a service: called web apps, or software-as-a-service. The twelve-factor app is a methodology for building software-as-a-service apps that:
* Use declarative formats for setup automation, to minimize time and cost for new developers joining the project.
* Have a clean contract with the underlying operating system, offering maximum portability between execution environments.
* Are suitable for deployment on modern cloud platforms, obviating the need for servers and system administration;
* Minimize divergence between development and production, enabling continuous deployment for maximum agility
* And can scale up without signification changes to tooling, architecture, or development practices
The twelve-factor methodology can be applied to apps written in any programming language, and which use any combination of backing (database, queue, memory cache, etc.)

## Background
The contributors to this document have been directly involved in the development and deployment of hundreds of apps, and indirectly witnessed the development, operation, and scaling of hundreds of thousands of apps via our work on the Heroku platform.
This document synthesizes all of our experience and observations on a wide variety of software-as-a-service apps in the wild. It is a triangulation on ideal practices for app development, paying particular attention to the dynamics of the organic growth of an app over time, the dynamics of collaboration between developers working on the app’s codebase, and avoiding the cost of software erosion.
Our motivation is to raise awareness of some systemic problems we’ve seen in modern application development, to provide a shared vocabulary for discussing those problems, and to offer a set of broad conceptual solutions to those problems with accompanying terminology. The format is inspired by Martin Fowler’s books Patterns of Enterprise Application Architecture and Refactoring.

## Who Should Read this Document?
Any developer building applications which run as a service. Ops engineers who deploy or manage such applications.

## 12 Factors
1. [Codebase](https://github.com/aindrajaya/twelve-factor/roles#1-codebase)
2. [Dependencies](https://github.com/aindrajaya/twelve-factor/roles#2-dependency)
3. [Config](https://github.com/aindrajaya/twelve-factor/roles#3-config)
4. [Backing Services](https://github.com/aindrajaya/twelve-factor/roles#4-backing-services)
5. [Build, release, run](https://github.com/aindrajaya/twelve-factor/roles#5-build-release-run)
6. [Processes](https://github.com/aindrajaya/twelve-factor/roles#6-processes)
7. [Port binding](https://github.com/aindrajaya/twelve-factor/roles#7-port-binding)
8. [Concurrency](https://github.com/aindrajaya/twelve-factor/roles#8-concurrency)
9. [Disposability](https://github.com/aindrajaya/twelve-factor/roles#9-disposability)
10. [Dev/Prod Parity](https://github.com/aindrajaya/twelve-factor/roles#10-dev-pro-parity)
11. [Logs](https://github.com/aindrajaya/twelve-factor/roles#11-logs)
12. [Admin Processe](https://github.com/aindrajaya/twelve-factor/roles#12-admin-processes)
