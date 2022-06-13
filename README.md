# .NET Microservice

 ### Things I'll Be Covering

#### Intro & Theory

- [ ] What are Microservices
- [ ] Our Services
- [ ] Solution & Architecture
- [ ] Service Architecture

#### Intro & Theory

- [ ] Overview
- [ ] Scaffolding
- [ ] Data Layering
- [ ] Controller & Actions

#### Docker & Kubernetes

- [ ] Review of Docker
- [ ] Intro to Kubernetes
- [ ] Kubernetes Architecture
- [ ] Deployment of Platform Service
- [ ] External Newtwork Access

#### Command Service

- [ ] Scaffolding
- [ ] Controlelr & Action Synchronous & Asynchronous Messaging
- [ ] Deploy service to Kubernetes
- [ ] Internal Networking
- [ ] API Gateway

#### SQL Server

- [ ] Persistent Volume Claims
- [ ] kubernetes Secrets
- [ ] Deploy SQL Sever To Kubernetes
- [ ] Revist Platform Service

#### Muli-Resource API

- [ ] Review Of Endpoints and Commands Service
- [ ] Data Layer
- [ ] Controllers & Actions

#### Message Bus / RABBITMQ

- [ ] Solution Architecture
- [ ] RabbitMQ Overview
- [ ] Delploy RabbitMQ to Kubernetes
- [ ] Test


#### Asynchronous Messaging

- [ ] Adding a Message Bus Publisher to Platform Service
- [ ] Event Proccesing
- [ ] Adding an Event Listener to the Command Service

#### GRPC

- [ ] Overview of GRPC
- [ ] Final Kubernetes networking
- [ ] Addinf gRPC server to Platform Service
- [ ] Creating a "proto" file
- [ ] Adding a gRPC client to the Commands Service
- [ ] Deploy & Test

# 1 Principles

#### Microserves are small ( Consider a team that would be able to eat to 2 pizzas pies and be satisfied another way to consider this would be a team that takes only 2 weeks to build it)

#### They are small and do they're jobs extremly well, they dont rely too much on other parts of the system. paradoxically in order for it to be a microserves, said services will have to talk to each other.

#### Form Part of the (distributed) whole
#### Self-contained / Autonomous

## Monoliths

#### Large monolithic CRM system are systems that:
- [ ] Service millions of customers
- [ ] Built over many years
- [ ] Built on a single, proprietary tech stack
- [ ] Usally "out-sourced" to 3rd parties

#### This causes for the system to be:
- [ ] Very difficult to change
- [ ] Change cycles are usally months in duration
- [ ] Massive ammounts of testing
- [ ] Difficult to scale
- [ ] Locked into technology stack

#### An example of this scale can be - you expirence increase orders on a holiday and you want to scale the part of the system that just deals with ordering and not really the other parts. You would need to scale the entire CRM.

# 2 Benifits of Microservices

- [ ] Easier to change & deploy (small and decoupled)
- [ ] Can be built using different technologies
- [ ] Increased ownership & alignment
- [ ] Extremely Resilient - 1 part of the service can break and the others will continue to run
- [ ] scaleability 
- [ ] Built to be highly replaceable / swappable

# 3 Disadvantages of Microservices

- [ ] Can be difficult to implement
- [ ] Need strong domain knowledge
- [ ] Distributed - a horror if there is a network fail / slow down

# 4 Advantages of Monoliths

- [ ] Simplier to implement
- [ ] Can use CI/CD, daily deploys, small changes
- [ ] Allows you to familiarise yourself with the domain ( this is benifitial to startups when they first begin created their domains )
- [ ] Might have a hybrid approach - can still build 2 or 3 big services without relative hardship
- [ ] Not as reliant on network
