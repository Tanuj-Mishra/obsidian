


# Quality Attributes, Requirements, and Architectural Styles

## Overview
- QAs are concerned with the qualities the system must exhibit, while architectural styles provide a methodology for achieving those qualities through design.
### Q1: What are quality attributes (QAs) in software architecture?
**A1:** Quality attributes are measurable or testable properties of a software system that indicate how well it meets stakeholder needs. They must be clear and objective to ensure well-defined and testable requirements.

### Q2: What role do architects play in relation to quality attributes?
**A2:** Architects translate quality attributes into concrete software structures and designs by choosing architectural styles and design elements that align with the desired quality attributes.
## Quality Attributes
### Q3: Why are quality attributes important in architecture?
**A3:** Quality attributes are critical for ensuring that the software architecture meets the functional and nonfunctional requirements of the system. They help determine the best architectural style for a given scenario.
### Q4: What is an example of a measurable requirement?
**A4:** A measurable functional requirement could be: "A user must be able to perform a certain task within four mouse clicks," as opposed to vague terms like "good" user interface.
## Architecturally Significant Quality Attributes

### Q5: How does architecture support quality attributes?
**A5:** Architecture translates nonfunctional requirements into underlying software structures, enabling the expression and achievement of desired qualities in a software system.

### Q6: What is a checklist of commonly encountered quality attributes?
**A6:** Common quality attributes include:
- Performance
- Scalability
- Availability
- Security
- Flexibility

## Important Quality Attributes

### Q7: What are some important quality attributes and how can they be tested?
- some unknown terms are there: latency, throughput, penetration testing, response time, etc.  

| **Quality Attribute** | **Description**                                                       | **How to Test It**                                                  |
|-----------------------|-----------------------------------------------------------------------|---------------------------------------------------------------------|
| Availability          | Proportion of time the system is operational                          | Measured as a percentage of downtime over a predefined period       |
| Maintainability       | Ability to undergo changes                                            | Measured by the time taken to implement required changes            |
| Performance           | Responsiveness of a system to execute commands                        | Measured in terms of latency or throughput                          |
| Reliability           | Chances of the product performing intended behavior                   | Measured by test-retest correlation scores                           |
| Reusability           | Usability of the product in producing other products                  | Tested by evaluating functionality in different scenarios           |
| Security              | Measures to protect the system from unauthorized access               | Tested via penetration testing, code reviews, and security assessments |
| Scalability           | System's capacity to increase or decrease capability                  | Measured by the ability to handle varying user requests             |
| Load balancing        | Technique to distribute workloads across resources                     | Evaluated by response time and resource utilization                  |
| Caching               | Temporary storage of frequently accessed data                          | Measured by hit rate, response time, and reduction of I/O operations |

## Requirements and Constraints

### Q8: What is the role of requirements in architecture?
**A8:** Requirements drive the architecture, ensuring that the software meets the needs of stakeholders while adhering to the real-world constraints that can impact the system.
### Q9: What are constraints in software architecture?
**A9:** Constraints are design decisions that cannot be compromised, influenced by external factors such as resource availability, time, budget, technology, and skill sets. They may conflict and require prioritization.
### Q10: Can you give an example of conflicting constraints in software design?
**A10:** In a ride-sharing application:
- **Real-time responsiveness:** Users expect instant updates, requiring low-latency communication.
- **Data security:** Strong security measures are essential to protect user data, which can introduce latency.
Balancing these constraints involves trade-offs where enhancing one may compromise the other.

## Architectural Styles

### Q11: What are architectural styles in software design?
**A11:** Architectural styles, or patterns, provide guidelines for designing software applications, including principles on component types, relationships, limitations on combinations, and expectations for how components interact.
### Q12: What factors influence the selection of an architectural style?
**A12:** The choice of architectural style depends on:
- Nature of the application (functional and nonfunctional requirements)
- Constraints (infrastructure limitations)
- Specific scenarios the application must accommodate

