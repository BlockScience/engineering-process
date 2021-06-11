# Work Breakdown Structure

This document is the first of four which will outline both the work required to complete economic engineering work as a general dynamic system successfully.

<!-- Create engineering parallel examples for each phase -->
<!-- Blow out not only phases but also radii, describing damage scenarios and analysis -->

![](https://i.imgur.com/mFAqCsE.png)
[Reference for image](https://direct.mit.edu/books/book/2908/Engineering-a-Safer-WorldSystems-Thinking-Applied)

## Phase 1 - Requirements (Bundles 1-3)
The first phase of a properly engineered system is the requirements phase. This phase takes a project from a set of business requirements, varying in maturity, and is completed when the requirements are sufficiently defined to begin the mathematical specification in the design phase of the engineering process.

### Bundle 1: Narrative Business Requirements

*  Collect Business Requirements
*  Resolve inconsistencies or disagreement with client team
*  Understand/Flag Legal & Regulatory Considerations
*  Technical (tools, platform) Considerations

**Document: Documented Narrative (e.g. User stories, Stated goals, etc.)**

### Bundle 2: Formal Requirements

*  Begin to translate Business Requirements into Formal Requirements
*  Utilize appropriate taxonomies, diagramming techniques, etc. to drive alignment and establish formal framework
   

**Document: Role & Fee Taxonomies, Entity Relationship Diagrams, Causal Loop Diagrams, Stock and Flow, etc.**

### Bundle 3: System Scoping

*  Scoping: break vision scope down in space and time
    * Space: subsystems and interfaces
    * Time: "as-is" -> "to be" system, matching vision and roadmap of client
    * Identify specific area (e.g. subsystem) of focus for design 
    
**Document: System Mapping(s), Roadmap, Identification of Scope for Design**

### Overall Phase Deliverable: System Requirements Report

## Phase 2 - Design (Bundles 4-6)

### Bundle 4: Spec Requirements

*  Scope Specific Economic Math Spec 
    * State space, $X$
    * Mechanism in domain-and-range form $f(X,u)= X^+$
    * Metrics defined in state space M(X)
    * Requirements defined using metrics

**Document: Concept Mathematical Specification**


### Bundle 5: Spec Design
The Concept Math Spec represents the formal mathematical requirements necessary for design. The Preliminary Math Spec starts from the foundation laid in the Concept Math Spec. The document of the Preliminary Math Spec with the Mechanism Specification should represent the current design and completion of the Design Phase of the engineering process. The delivered document is defined to the level to build a cadCAD model and specify an implementation guide.
Any information in the Concept Math Spec that will help explain the design can be merged into the Preliminary Math Spec, with the important caveat that merge conflicts are resolved with the Preliminary Math Spec superseding.

* Scope Specific Economic Mathematical Specification (Design Phase)
    * Define function in mechanism specification which meets the requirements
    * Analytic verification that the design meets the requirements
    * Define User Action space $u$ mapped across $f(X,u)$
    
**Document: Preliminary Mathematical Specification**


### Bundle 6: Model Development

* cadCAD model development
* Convert math specs into python repositories that allow computational tests
    * Define system model boundary
    * Specify data model of state
    * Numerical verification test mechanisms 
    * Determine local state for agents
    * Numerical verification test agent state
    
**Document: Model Source Code, Test Results and Analysis**

### Overall Phase Deliverable: Math Specs and cadCAD Model

## Phase 3 - Validation (Bundles 7-8)
### Bundle 7: Model Evaluation

* System Integration Testing
    * cadCAD model test mechanism interaction
    * cadCAD model test agent dynamics
    * 
**Document: Model Source Code, Test Results and Analysis**

### Bundle 8: Scenario Evaluation

* scenario testing using cadCAD model
    * computational experiments to evaluate scenarios and/or turn params
    * ...

### Overall Phase Deliverable: Validated cadCAD Model and Parameter Selection

## Phase 4 - Implementation and Operationalization (Bundles 9-11)
### Bundle 9: Model Integration

* feed models with data from real life (batch style)
    * ... data science work


### Bundle 10: Model Operation

* operationalize models for ongoing monitoring and maintainence
    * ... productionalization of data science work

### Bundle 11: Decisions Through Models

* "computer aided governance"
    * people can combine their intuitions with counterfactual scenarios to form more informed opinions about alternative mechanism parameters, or entirely new policies that can be added or swapped for existing ones.



---
## References
1. https://direct.mit.edu/books/book/2908/Engineering-a-Safer-WorldSystems-Thinking-Applied