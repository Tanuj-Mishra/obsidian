
                        n

# Types of Architecture Patterns



## Overview

### Q: What are the three categories of structures in architectural design?
- There are three different categories of structures in architectural design, although they highlight different aspects of the same design.
- The three categories are:
	1. Static or _module structures_
	2. Dynamic structures (_component and connector structures_)
	3. Deployment structures (_allocation structures_)
## Static Structures
### Q: What is the main objective of static structures?
The main objective is to assign different areas of functional responsibility and discuss how the system is structured based on code.
### Q: What are the key components of static structures?  
The key components include:
-  **Decomposition:** 
	- Larger and more complex modules are divided into smaller and easily manageable modules.
	- They essentially follow a top-down approach: we start with one big module, discussing all the tasks that our system has to do, and then we decompose modules into sub-modules based on different functionalities
- **Uses:** 
	- Describing the relationship between modules[i.e. uses relation], indicating whether one module uses another, this allows incremental development of the software.
- **Layered Architecture:** 
	- Organizing functions into layers that hide implementation details from higher layers.
	- In essence, by controlling which layers use which services, you organize your software into **distinct levels**, each focused on a specific task, leading to a more structured and maintainable architecture.
	- ![[layered-architecture-diagram.png]]
		- A layer N can only access the services offered by layer N - 1.
- **Class Structure:** 
	- Defining module units as classes on which inheritance and composition relationships are defined.
	- Benefits
		- Reuse different components of classes.
		- also helps in incremental development by adding functionality in incremental way.



## resume from here after





## Dynamic Structures

### Q: What do dynamic structures explain?
Dynamic structures explain how the system is constructed as a collection of elements with runtime behavior (components) and interaction (connectors).
### Q: What are the components of dynamic structures?
The components include:
- **Communication Process:** Handling dynamic characteristics through synchronization and communication.
- **Concurrency:** Exploring opportunities for parallelism and managing concurrency-related issues.
- **Shared Data:** Showing how data is produced, processed, and consumed by different modules.
- **Client-Server:** Describing interactions between clients and servers through messages and protocols.
## Deployment Structures
### Q: What do deployment structures describe? 
Deployment structures describe how the system interacts with non-software structures and depict interactions between software elements and external environments.
### Q: What are the components of deployment structures?
The components include:
- **Deployment:** How software components interact with hardware and communication elements.
- **Implementation:** How different software components integrate with file structures.
- **Work Assignment:** Assigning implementation and integration details to appropriate development teams.
## Conclusion
### Q: How are architectural patterns classified?
Architectural patterns can be classified based on the predominant type of components they display:
- **Module patterns:** Depict modules.
- **Component and connection patterns:** Depict components and connectors.
- **Allocation patterns:** Depict software elements and non-software elements.
### Q: What is noteworthy about the focus of literature on architectural patterns?
Most literature focuses on component and connector patterns, but module patterns and allocation patterns also exist. Different patterns provide various angles of the same system, allowing an architectural style to be classified in multiple ways.


## Questions
1. What is structure in terms of architectural pattern or classification done above.