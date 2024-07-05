# SLV04b Logical Internal Exchange VP

## Purpose
The Logical Internal Exchange Viewpoint serves for the identification and definition of interfaces of elements of the logical system. also, the delegation of system element interfaces to the logical system boundary interfaces is covered. The Logical Internal Exchange Viewpoint
* identifies system element interfaces on a logical level
* states to which other logical elements the interfaces are connected to
* assigns conceptual interface definitions to interfaces
* defines the usage of interfaces, e.g., if only a subset of the interfaces is used
* defines the delegation of logical system element interfaces to the logical system boundary interfaces

## Example

## Workflow
**Viewpoint Input:**
* instantiated Logical Internal Roles within the Logical SOI from [SLV02a](Logical-Structure-Definition-Viewpoint.md)
* SAF_DomainItemKind as exchange items between Logical Internal Roles from [SFV02a](System-Domain-Item-Kind-Viewpoint.md)
* SAF_ConceptualInterfaceDefinition from [SFV05a](System-Interface-Definition-Viewpoint.md) to formalize SoI's external interfaces.
* itemFlows from [SLV04a](Logical-Internal-Interaction-Viewpoint.md) and [SFV03c](System-Functional-Refinement-Viewpoint.md)

**Step-by-Step Guide:**
1.	Select the Logical SOI and add a new Logical Internal Exchange Diagram as a specialized [SysML1.5 Internal Block Diagram](https://sparxsystems.com/enterprise_architect_user_guide/16.1/modeling_languages/internal_block_diagram.html) with Add Diagram > SAF > InternalBlock > SAF::SLV04b_SystemInternalExchangeView.
2.	Drag and drop the involved Logical Internal Roles from the Logical SOI onto the System Internal Exchange Diagram.
3.	Add new required interfaces as Proxy Ports to the Logical Internal Role or select the needed required Proxy Ports from the property’s Feature Page > Interaction Points.
4.	For new Proxy Ports select or create an SAF_ConceptualInterfaceDefinition by selecting the Proxy Port > Properties > Property > Define > Type > Select Type ...
5.	In case of typed Proxy Ports set one interface side conjugated (propterties > element).
6.	If needed add FlowProperties to the SAF_ConceptualInterfaceDefinition to refine the interface or visualize a direction.
7.	Create a connector between the Logical Internal Role’s Proxy Port. Connect internal to external interfaces of the Logical SOI.
8.	If the Logical Internal Roles exchange information, energy, or material establish an Item Flow and select the according Domain Kind. Select the Connector > right-click on the Connector > Advanced > Information Flow Realized > Select the Domain Kind(s)

**Viewpoint Output:**
* ItemFlows established can be reused in [SFV03c](System-Functional-Refinement-Viewpoint.md) and [SLV04a](System-Internal-Interaction-Viewpoint.md)

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* Connector
* FlowProperty
* ItemFlow
* ProxyPort
* [SAF_ConceptualInterfaceDefinition](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_ConceptualInterfaceDefinition)
* [SAF_DomainKind](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_DomainKind)
* [SAF_LogicalElement](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_LogicalElement)

## General Recommendations and Pitfalls
* It is required that the exchanges in [SLV04a](Logical-Internal-Interaction-Viewpoint.md), [SFV03c](System-Functional-Refinement-Viewpoint.md) are addressed in this diagram to ensure consistency.

[>>> back to cheat sheet overview](../CheatSheet.md)
