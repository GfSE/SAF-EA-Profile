# SPV01b Physical Context Definition VP

## Purpose
The Physical Context Definition Viewpoint identifies the various contexts the SOI is used in, along with the associated external entities sharing a physical interface with the system. For each context, the applicable environmental conditions shall be defined. The physical context helps identify the interface requirements needed to integrate a system into its environment in a given context.

## Example

## Workflow
**Viewpoint Input:**
* N/A

**Step-by-Step Guide:**
1.	Create a new Physical Context Definition diagram as specialized [SysML1.5 Block Definition Diagram](https://sparxsystems.com/enterprise_architect_user_guide/16.1/modeling_languages/block_definition_diagrams.html) in the dedicated package in your model with Add Diagram > SAF > BlockDefinition > SAF::SPV01b_PhysicalContextDefinitionView.
2.	Create a Physical System Context to the diagram.
3.	Create a Physical System and Physical Context Elements (e.g., a Physical User, Physical External System, or the Physical Environment).
4.	Create Physical Context Roles by using the composition relationship.
5.	Give the Physical Context Role a meaningful name by selecting the part property in the Physical Context and amending the name on the property element page for traceability purposes in matrix specifications. 
6.	If needed, define the multiplicity for the Physical Context Roles.

**Viewpoint Output:**
* Physical System to all futher viewpoints in the Physical Domain
* the Physical Context Roles used in viewpoints [SPV01c](Physical-Context-Exchange-Viewpoint.md)

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* [SAF_PhysicalContextRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalcontextrole) contained in SAF_PhysicalContext
* [SAF_PhysicalContext](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalcontext)
* [SAF_PhysicalEnvironment](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalenvironment)
* [SAF_PhysicalExternalSystem](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalexternalsystem)
* [SAF_PhysicalSystem](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalsystem)
* [SAF_PhysicalUser](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicaluser)

## General Recommendations and Pitfalls
* Name the properties as for traceability management in Enterprise Architect the matrix specification displays the element name only.
* At least one Physical Context is required for a model. It is possible however, to create several Physical Contexts with different scopes (physical configurations). However, a holistic system context view has to be created.

[>>> back to cheat sheet overview](../CheatSheet.md)
