# SPV04b Physical Internal Exchange VP

## Purpose
The Physical Internal Exchange Viewpoint serves for the identification and definition of interfaces of elements of the physical system. also, the delegation of system element interfaces to the physical system boundary interfaces is covered. The Physical Internal Exchange Viewpoint
* identifies system element interfaces on a physical level
* states to which other physical elements the interfaces are connected to
* assigns physical interface definitions to interfaces
* defines the usage of interfaces, e.g., if only a subset of the interfaces is used
* defines the delegation of physical system element interfaces to physical system boundary interfaces

## Example

## Workflow
**Viewpoint Input:**
* instantiated Physical Internal Roles within the Physical System from [SPV02a](Physical-Structure-Definition-Viewpoint.md)
* SAF_DomainItemKind as exchange items between Physical Internal Roles from [SFV02a](System-Domain-Item-Kind-Viewpoint.md)
* SAF_PhysicalInterfaceDefinition from [SFV05a](Physical-Interface-Definition-Viewpoint.md) to formalize Physical System's external interfaces.

**Step-by-Step Guide:**
1. Select the Physical System and add a new Physical Internal Exchange Diagram as a specialized [SysML1.5 Internal Block Diagram](https://sparxsystems.com/enterprise_architect_user_guide/16.1/modeling_languages/internal_block_diagram.html) with Add Diagram > SAF > InternalBlock > SAF::SPV04b_PhysicalInternalExchangeView.
2.	Drag and drop the involved Physical Internal Roles from the Physical System onto the Physical Internal Exchange Diagram.
3.	Add new required interfaces as Proxy Ports to the Physical Internal Role or select the needed required Proxy Ports from the property’s Feature Page > Interaction Points.
4.	For new Proxy Ports select or create an SAF_PhysicalInterfaceDefinition by selecting the Proxy Port > Properties > Property > Define > Type > Select Type ...
5.	In case of typed Proxy Ports set one interface side conjugated (propterties > element).
6.	Create a connector between the Physical Internal Role’s Proxy Port. Connect internal to external interfaces of the Physical System.
7.	If the created interfaces have an inherent dependency (such as pins, electrics, data protocol) model them separatly and set an InterfaceLayerRelationship.
8.	If the Physical Internal Roles exchange information, energy, or material establish an Item Flow and select the according Domain Kind. Select the Connector > right-click on the Connector > Advanced > Information Flow Realized > Select the Domain Kind(s)

**Viewpoint Output:**
* N/A 

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* Connector
* FlowProperty
* ItemFlow
* ProxyPort
* [SAF_PhysicalInternalRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalinternalrole)
* [SAF_InterfaceLayerRelationship](https://saf.gfse.org/userdoc/stereotypes.html#saf_interfacelayerrelationship)
* [SAF_PhysicalExchangeType](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalexchangetype)
* [SAF_PhysicalInterfaceDefinition](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalinterfacedefinition)

## General Recommendations and Pitfalls
* Complex interfaces have various aspects to address in an exchange diagram. SAF propagates a separate interface aspect handling which are coupled with the InterfaceLayerRelationship stereotyped relationship. This is to avoid excessive port nesting for more complex interfaces (Tower of Hanoi / Towers of Bramha syndrome).
* Create the interfaces of the Physical System as they are existing in real-world (as-build) - as-planned is scope of the Functional Domain.
* In Physical Domain all proxyPorts have to be classified by an SAF_PhysicalInterfaceDefinition.

[>>> back to cheat sheet overview](../CheatSheet.md)
