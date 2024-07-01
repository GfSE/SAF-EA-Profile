# SOV02c Operational Capability VP

## Purpose
The Operational Capability Viewpoint defines a taxonomy of Capabilities from a Stakeholder’s perspective including composition, specialization, and dependency relationships between Operational Capabilities.

## Example

## Workflow
Viewpoint Input:
* N/A

Step-by-Step Guide:
1.	Create a new Operational Capability Diagram in the dedicated package in your model as specialized SysML1.5 Block Definition Diagram with Add Diagram > SAF > BlockDefinition > SAF::SOV02c_OperationalCapabilityView.
2.	Add new Operational Capabilities on the diagram.
3.	Define Operational Capability Composition, Generalization and Dependencies between them. Please note that the composition must be set from parent to child.

Viewpoint Output:
* Operational Capabilities are in input for Stakeholder Requirements (SOV06a) and System Capabilities (SFV02b) which are contributing to Operational Capabilities.

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* [SAF_OperationalCapability](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalCapability)
* [SAF_OperationalCapabilityComposition](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalCapabilityComposition)
* [SAF_OperationalCapabilityDependency](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalCapabilityDependency)
* [SAF_OperationalCapabilityGeneralization](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalCapabilityGeneralization)

## General Recommendations and Pitfalls
* It is not necessarily required to define Operational Capabilities for a project. However, there are other frameworks (such as UAF) that integrate this step and build further development on these capabilities. If Operational Capabilities are used in the development process, they should be defined as per this viewpoint.
*	It is important to link Operational Capabilities to Operational Stories, Operational Interactions and/or Operational Processes to aide ensuring that the sum of the linked Operational Capabilities fully realize these. This process is not automized and not supported by the tool but must be ensured through reviews. Please note also SOV08b.
