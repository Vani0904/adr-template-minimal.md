# Decision 1
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

# Decision 2
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
  
# Decision 3
Security Considerations

## Context and Problem Statement

The CMS requires secure authentication and authorization to ensure that only valid users can log in and access permitted functionality. These roles include Consumer, Help Desk Agent, Help Desk Manager, and System Administrator.

## Considered Options

* Custom PHP Auth logic within controllers
* Laravel Middleware (Auth + Role)
* JWT Token-based authentication
* OAuth 2.0 / Single Sign-On

## Decision Outcome

Chosen option: "Laravel Middleware", because Laravel's Auth and Middleware system ensures only logged in users can access the CMS and that checks will be constantly put in place to confirm user roles for RBAC enforcement.

### Consequences

* Good, because easier to develop due to having the support for session-based auth in the framework.
  
* Bad, because session-based model may be less ideal for large distributed systems.

# Decision 4
Technology Stack Decisions (Revised)

## Context and Problem Statement

The Complaint Management System needs a working proof of concept (POC) that demonstrates the core system functions. With the Technology stack being quick to develop and easy to deploy locally and align with the monolithic architecture.

## Considered Options

* PHP (Laravel) + NoSQL (MongoDB)
* PHP (Laravel) + Sqlite
  
## Decision Outcome

Chosen option: "PHP (Laravel) + Sqlite", due to in the scope of my PoC, it seemed like the more suitable option over NoSQL having a more structured data compared to NoSQL
### Consequences

* Good, because the use of a Framework and a structured database can speed up the development of a prototype and the use of the Built-in Laravel Auth can simplify RBAC whilst still aligning with a monilithic design.
  
* Bad, because the use of NoSQL may limit the use of complex relational queries and lacks the scalability requirements of a fully functional version of the system.
# Decision 5

# Decision 6

