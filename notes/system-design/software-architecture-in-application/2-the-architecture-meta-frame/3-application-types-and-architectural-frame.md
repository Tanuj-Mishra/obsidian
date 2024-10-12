
- **Application types** focus on the fundamental approaches for designing applications, driving decisions based on specific user needs and technological constraints.
- **Architectural styles** provide structured guidelines for how those applications are built, emphasizing consistency and organization in the software design process.
___



## Application Types

#### Q1: What are application types in software architecture?
**A1:** Application types represent different fundamental approaches or paradigms for designing and structuring software applications. They provide a high-level understanding of how an application is built and influence architectural decisions.

#### Q2: How do application types drive architectural decisions?
**A2:** The selection of an application type is influenced by technological limits and the intended user experience. Choosing the appropriate application type is crucial for effective application creation and architecture.

#### Q3: What are some common application types and their requirements/constraints?

| **Application Type**   | **Requirements and Constraints**                                                                                           |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **Mobile Apps**        | Developed as web or rich client apps; support occasionally connected scenarios; run on devices with limited resources.     |
| **Rich Client Apps**   | Stand-alone applications; support disconnected scenarios; utilize local processing and storage resources.                  |
| **Rich Internet Apps** | Support multiple platforms/browsers; deployed over the internet; designed for rich media; run in the browser for security. |
| **Service Apps**       | Support multiple platforms/browsers; only connected scenarios; utilize server resources.                                   |
| **Web Apps**           | Support multiple platforms/browsers; only connected scenarios; utilize server resources.                                   |

___
### Deployment Strategy

#### Q4: How are application types and deployment strategies related?
**A4:** The choice of deployment strategy is influenced by factors such as the application's nature, requirements, scalability needs, and the architectural style being employed.

#### Q5: What is the difference between monolithic applications and microservices architecture regarding deployment?
**A5:** Monolithic applications have a single, self-contained deployment unit, making deployment straightforward. In contrast, microservices architecture involves multiple services that need to be independently deployed.

#### Q6: What should be considered during the design process regarding deployment strategies?
**A6:** Early identification of requirements and restrictions is crucial to choose a relevant deployment strategy and resolve conflicts between the application and infrastructure.

## Architecture Frame

### Q7: What is the architecture frame within the architecture meta-frame?
**A7:** The architecture frame is a collection of hotspots used to analyze application structure, allowing for the conversion of primary functions (e.g., caching, data access, validation) into actionable design decisions.

## Cross Cutting Concerns

### Q8: What are cross-cutting concerns in software design?
**A8:** Cross-cutting concerns are design aspects not tied to a single layer in the application. They address issues that affect multiple layers, such as authentication, caching, communication, and exception management.

### Q9: What are some important cross-cutting concerns?

| **Cross-Cutting Concern**      | **Description**                                                                                             |
|--------------------------------|-------------------------------------------------------------------------------------------------------------|
| **Authentication and Authorization** | Identifies users and determines access to resources; ensures proper granularity across layers.   |
| **Caching**                   | Improves performance and reduces server round-trips; identifies what and where to cache.                     |
| **Communication**             | Determines communication strategies between layers, including protocols and security.                        |
| **Exception Management**       | Handles errors without revealing sensitive information; includes error logging and user notifications.       |
| **Instrumentation and Logging**| Strategies for logging key events and maintaining an audit trail for security and recovery.                 |
| **Concurrency and Transaction**| Manages conflicts from multiple users; ensures multi-step operations are treated atomically.                |
| **Data Access**               | Techniques for abstracting and accessing data in the data store, including connection management.            |
| **User Experience (UX)**      | Interaction between users and the application; affects efficiency and user retention.                        |

