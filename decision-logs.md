# Week 2
Architecture Style Decision

## Context and Problem Statement

ABC Limited needs a scalable Complaint Management System for large clients such as banks and telecom companies. An initial architecture that supports this should be decided. Should the CMS start as a monolithic or a microservice-based sytem?

## Considered Options

* Monolithic Architecture
* Microservices Architecture
* Layered Modular Architecture

## Decision Outcome

Chosen option: "Monolithic Architecture", because it simplifies early development, speeds up the delivery of the proof of concept phase and meets the limited scalability requirements at this stage.

### Consequences

* Good, because it can make debugging and testing easier.
* Bad, because it has Limited scalability and will impact the system as the user base grows.

# Week 3
Technology Stack Decisions

## Context and Problem Statement

The Complaint Management System needs a working proof of concept (POC) that demonstrates the core system functions. With the Technology stack being quick to develop and easy to deploy locally and align with the monolithic architecture.

## Considered Options

* PHP (Laravel) + NoSQL (MongoDB)
* Node.js (Express) + MongoDB
* C# + MySQL

## Decision Outcome

Chosen option: "PHP (Laravel) + NoSQL (MongoDB)", because Laravel can provide the authentication and RBAC support required aligning with the security requirements of the system. A NoSQL backend such as MongoDB provides a flexible schema design which speeds up the initial develoipment and testing phases of a new system.

### Consequences

* Good, because the use of a Framework and Lightweight Database can speed up the development of a prototype and the use of the Built-in Laravel Auth can simplify RBAC whilst still aligning with a monilithic design.
  
* Bad, because the use of NoSQL may limit the use of complex relational queries and lacks the scalability requirements of a fully functional version of the system.
  
# Week 4
{Title}
## Context and Problem Statement

The Complaint Management System needs a working proof of concept (POC) that demonstrates the core system functions. With the Technology stack being quick to develop and easy to deploy locally and align with the monolithic architecture.

## Considered Options

* PHP (Laravel) + NoSQL (MongoDB)
* Node.js (Express) + MongoDB
* C# + MySQL

## Decision Outcome

Chosen option: "PHP (Laravel) + NoSQL (MongoDB)", because Laravel can provide the authentication and RBAC support required aligning with the security requirements of the system. A NoSQL backend such as MongoDB provides a flexible schema design which speeds up the initial develoipment and testing phases of a new system.

### Consequences

* Good, because {positive consequence, e.g., improvement of one or more desired qualities, …}
* Bad, because {negative consequence, e.g., compromising one or more desired qualities, …}
* … <!-- numbers of consequences can vary -->
# Week 5

# Week 6

# Week 7

# Week 8

# Week 9

# Week 10
