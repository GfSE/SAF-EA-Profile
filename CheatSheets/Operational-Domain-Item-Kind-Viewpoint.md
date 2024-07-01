# SOV02a Operational Domain Item Kind VP

## Purpose
The Operational Domain Item Kind Viewpoint captures enterprise wide concepts and collects type definitions for any exchanged item of the Operational Domain. Its purpose is to define these item types and their relationships.

## Example

## Workflow
Viewpoint Input:
* N/A

Step-by-Step Guide:
1.	Create a new Operational Domain Kind diagram as specialized SysML1.5 Block Definition Diagram with Add Diagram > SAF > BlockDefinition > SAF_SOV02a_OperationalDomainKindView.
2.	Create new Operational Domain Kind which is required to describe an exchange of information, energy, or material between Operational Roles.
3.	If needed, you can formalize the Domain Kind attributes with value types or enumerations.
4.	If needed, you can establish an Operational Domain Kind Composition relationship between two Operational Domain Kinds. Please note that the composition must be set from parent to child.

Viewpoint Output:
* Operational Domain Items Kinds as item to exchange in operational context exchanges (SOV01c), operational processes (SOV03a) or operational interactions (SOV04a).

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* [SAF_OperationalDomainKindComposition](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalDomainKindComposition)
* [SAF_OperationalDomainKind](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalDomainKind)

## General Recommendations and Pitfalls
* It is recommended to define Operational Domain Kinds only in this viewpoint.
* For a common understanding of the different Operational Domain Kinds, it is helpful to provide written information on it. This is best done through a rationale for each Operational Domain Kind.
* There should only be one Operational Domain Item Kind Viewpoint for the overall project.
* For overview purposes it is recommended to display the diagram in specification view.
