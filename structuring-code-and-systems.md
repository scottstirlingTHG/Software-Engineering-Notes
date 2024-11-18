# Structuring code and systems notes

In these notes I am planning on disucssing the microservice model and I plan on contrasting that with the monolith archtitecture.


## Monoliths

Before discussing microservices we will discuss what kind of software we are currently most familiar with (at least in terms of coding); this is the most traditional type of software, the Monolith architecture. 

This is a singular (often large) code base that couples all of the business concerns together where it would be manipulating a single database. This comes with all sorts of problems:

- slower development speed - A larg monolithic application make development more complex and slower.

- Not amenable to multiple teams - It can be difficult to have multiple teams working concurrently to add new features in the same application when it is a monolith (especially when compared to microservices).

- Scalability - It is difficult to scale individual components.

- Reliability - A single point of failure in the code could bring the entire application down.

- Difficult to adopt new tech - any changes in framework or language would require large rewrites.

- Deployment - When making a small change have to redeploy the whole application which can be time consuming.

These problems are intended to be solved by Microservices.

## Microservice Architecture

A Microservice Architecture (commonly called microservices) in contrast to the monolith where everything is more tightly coupled you instead have a an application made out of many smaller components (services). These services normally only have one specialised function. These services all operate independently of one another so there is much looser coupling of the components which grants all the following benifits.

These are the following benefits of microservices:

- Services are independently deployable - since each microservice is independent of the others they can be depoloyed withouy interacting with the rest of the application.

- Multiple language use - with microservices you can build an application using multiple languages allowing teams to have greater flexibility in what tools they use.

- Consumability -  Each service can be consumed by multiple services without strict coupling.

- Scalability - As they are made of smaller parts a microservice architecture is much easier to sclae than an applications using a monolith architecture.

- Can have a higher performance speed.

As you can see a lot of the features of microservices directly combat some of the drawbacks of a monolithic architecture.
## Drawbacks of Mircorservices

These are some of the drawbacks of a microservice architecture:

- Increased complexity - Microservices lead to more complexity compared to a monalith and could lead to development sprawl.

- Higher infrastructure costs - each new service needs new test suites, deployment playbooks hosting infrastructure.

- Difficult to debug - each microservice has its own logs and can make debugging more complicated.

-Network latency - since request to various services have to be sent over a network to get to the client the speed of the network can be a significant bottle neck for the speed of the application.

- Lack of standardardisation - each team managing a service may have different standards comapred to the other teams.

## Where is microservice architecture used?

Here are some of the companies (Other than THG) that use a Microservice architecture:

- Amazon

- Uber 

- Netflix 

## Bibliography

- https://www.atlassian.com/microservices/microservices-architecture/microservices-vs-monolith

- https://www.mulesoft.com/api/microservices/monolithic-vs-microservices

