# SAF Cheat Sheets for EA

Welcome to the cheat sheet library for the EA implementation of SAF. You can find for each viewpoint a helping one pager which helps you to master SAF in your daily working life in Sparx Enterprise Architect.
Each cheat sheets consists of:
* a short purpose explaination of the viewpoint
* an example how the diagrams could look like in EA (FFDS example)
* step-by-step work-flow
* exposed elements in the specific viewpoint
* general recommendations and common pitfalls observed.

## Viewpoints Operational Domain

The SAF Operational Domain aims to get an understanding of required organizational or operational entity capabilities, as a foundation and reasoning for to systems to be acquired or developed. The SAF Operational Domain supports the model-based development of a [CONOPS](https://www.sebokwiki.org/wiki/Concept_of_Operations_(ConOps)_(glossary)) - as well as an [OPSCON](https://www.sebokwiki.org/wiki/Business_or_Mission_Analysis) and related life cycle concepts - for an organization or operational entity seeking for an improvement of existing capabilities or in establishing new ones. By identifying Stakeholders and their Requirements the SAF Operational Domain supports the derivation of a complete and consolidated set of Stakeholder Requirements based on operational stories, operational processes, operational capabilities, and operational exchanges.

Available sheets operational domain:
* [SOV01a Operational Story Viewpoint](CheatSheets/Operational-Story-Viewpoint.md)
* [SOV01b Operational Context Definition Viewpoint](CheatSheets/Operational-Context-Definition-Viewpoint.md)
* [SOV01c Operational Context Exchange Viewpoint](CheatSheets/Operational-Context-Exchange-Viewpoint.md)
* [SOV02a Operational Domain Item Kind Viewpoint](CheatSheets/Operational-Domain-Item-Kind-Viewpoint.md)
* [SOV02b Operational Performer Viewpoint](CheatSheets/Operational-Performer-Viewpoint.md)
* [SOV02c Operational Capability Viewpoint](CheatSheets/Operational-Capability-Viewpoint.md)
* [SOV02d Stakeholder Identification Viewpoint](CheatSheets/Stakeholder-Identification-Viewpoint.md)
* [SOV03a Operational Process Viewpoint](CheatSheets/Operational-Process-Viewpoint.md)
* [SOV04a Operational Interaction Viewpoint](CheatSheets/Operational-Interaction-Viewpoint.md)
* [SOV06a Stakeholder Requirement Viewpoint](CheatSheets/Stakeholder-Requirements-Viewpoint.md)
* [SOV08a Operational Capability Mapping Viewpoint](CheatSheets/Operational-Capability-Mapping-Viewpoint.md)
* [SOV08b Operational Process Mapping Viewpoint](CheatSheets/Operational-Process-Mapping-Viewpoint.md)

## Viewpoints Functional Domain

The SAF Functional Domain assumes a conceptual black box perspective onto the system to be developed. It translates Operational Domain usage into the notion of System Functions defining the demanded system behavior and quality attributes - performance, safety, security, etc.; the demanded system behavior as it is perceived by the User or other Entities at the System Boundary (known as usage behavior). The result of the elaboration of the viewpoints in the Functional Domain is a comprehensive System Specification.

Available sheets operational domain:
* [SFV01a System Use Case Viewpoint](CheatSheets/System-Use-Case-Viewpoint.md)
* [SFV01b System Context Definition Viewpoint](CheatSheets/System-Context-Definition-Viewpoint.md)
* [SFV01c System Context Exchange Viewpoint](CheatSheets/System-Context-Exchange-Viewpoint.md)
* [SFV02a System Domain Item Kind Viewpoint](CheatSheets/System-Domain-Item-Kind-Viewpoint.md)
* [SFV02b System Capability Viewpoint](CheatSheets/System-Capability-Viewpoint.md)
* [SFV02c System Functional Breakdown Viewpoint](CheatSheets/System-Functional-Breakdown-Viewpoint.md)
* [SFV03a System Process Viewpoint](CheatSheets/System-Process-Viewpoint.md)
* [SFV03b System State Viewpoint](CheatSheets/System-State-Viewpoint.md)
* [SFV03c System Functional Refinement Viewpoint](CheatSheets/System-Functional-Refinement-Viewpoint.md)
* [SFV04a System Context Interaction Viewpoint](CheatSheets/System-Context-Interaction-Viewpoint.md)
* [SFV05a System Interface Definition Viewpoint](CheatSheets/System-Interface-Definition-Viewpoint.md)
* [SFV06a System Requirement Viewpoint](CheatSheets/System-Requirement-Viewpoint.md)
* [SFV08a System Capability Mapping Viewpoint](CheatSheets/System-Capability-Mapping-Viewpoint.md)
* [SFV08b System Requirement Traceability Viewpoint](CheatSheets/System-Requirement-Traceability-Viewpoint.md)

## Viewpoints Logical Domain

The SAF Logical Domain assume a conceptual white box perspective onto the system to be developed. The Logical Domain Viewpoints describe the Logical Structure and the distribution of responsibilities for the Functionality of the SOI by means of a network of interacting Logical Elements that are responsible for a set of desired Functions. These Logical Elements and their Interactions are arranged in the Logical Architecture of the SOI. The structure of the Logical Architecture is in general influenced by nonfunctional criteria, e.g., maintainability, safety, and reliability. The Logical Domain is not a different abstraction level - compared to the Functional Domain, but a white box perspective on the same abstraction level.

Coming soon.

## Viewpoints Physical Domain

The SAF Physical Domain diagrams may be used to represent the Product Breakdown Structure, to identify external and internal physical interfaces, to provide diagrams for the system overview, to support the integration planning, to support production planning and to depict the features and variations implied in the system. The physical architecture typically is a combination of re-use elements, COTS elements and make-items for HW as well as for SW. The properties of the selected physical components and their provided resources are identified and modelled. A major concern of the Physical Domain are the physical interfaces, their identification and definition. For that purpose, the Physical Domain provides the diagrams to model interface with different level of detail considering the actual needs for the point of time in the project life cycle. For traceability the Physical Domain defines diagrams showing the mapping of the functional elements and their interfaces to physical elements and their interfaces.

Coming soon.

## Viewpoints Common Domain

The SAF Common Domain provides viewpoints addressing model information that is common to all other domains or that are applicable throughout the model.

Coming soon.
