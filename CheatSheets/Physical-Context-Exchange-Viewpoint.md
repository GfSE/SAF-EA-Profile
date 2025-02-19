# SPV01c Physical Context Exchange VP

## Purpose
The Physical Context Exchange Viewpoint focuses on the identification of the physical interfaces with external entities and relevant documentation. It is used to capture interface design requirements, applicable standards, protocols and format specifications, that are agreed upon the interfaces.

## Example

## Workflow
**Viewpoint Input:**
* instantiated Physical Context Roles within the Physical Context from [SPV01b](Physical-Context-Definition-Viewpoint.md)
* SAF_DomainItemKind as exchange items between Physical Context Roles from [SFV02a](System-Domain-Item-Kind-Viewpoint.md)
* SAF_PhysicalInterfaceDefinition from [SPV05a](Physical-Interface-Definition-Viewpoint.md) to formalize Physical System's external interfaces.

**Step-by-Step Guide:**
1.	Select a Physical Context and add a new Physical Context Exchange Diagram as a specialized [SysML1.5 Internal Block Diagram](https://sparxsystems.com/enterprise_architect_user_guide/16.1/modeling_languages/internal_block_diagram.html) with Add Diagram > SAF > InternalBlock > SAF::SPV01c_PhysicalContextExchangeView.
2.	Drag and drop the involved Physical Context Roles from the Physical Context onto the Physical Context Exchange Diagram.
3.	Add new required interfaces as Proxy Ports to the Physical Context Role or select the needed required Proxy Ports from the property’s Feature Page > Interaction Points.
4.	For new Proxy Ports select or create an SAF_PhysicalInterfaceDefinition by selecting the Proxy Port > Properties > Property > Define > Type > Select Type ...
5.	In case of typed Proxy Ports set one interface side conjugated (propterties > element).
6.	Create a connector between the Proxy Ports of Physical Context Roles.
7.	If the created interfaces have an inherent dependency (such as pins, electrics, data protocol) model them separatly and set an InterfaceLayerRelationship.
8.	If the Physical Context Roles exchange specific information, energy, or material establish an Item Flow and select the according Domain Kind. Select the Connector > right-click on the Connector > Advanced > Information Flow Realized > Select the Domain Kind(s)

**Viewpoint Output:**
* external Interfaces as ProxyPorts can be reused in [SPV04b](Physical-Internal-Exchange-Viewpoint.md)

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* Connector
* FlowProperty
* ItemFlow
* ProxyPort
* [SAF_PhysicalContextRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalcontextrole)
* [SAF_InterfaceLayerRelationship](https://saf.gfse.org/userdoc/stereotypes.html#saf_interfacelayerrelationship)
* [SAF_PhysicalExchangeType](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalexchangetype)
* [SAF_PhysicalInterfaceDefinition](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalinterfacedefinition)
* [SAF_PhysicalSystem](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalsystem)

## General Recommendations and Pitfalls
* Complex interfaces have various aspects to address in an exchange diagram. SAF propagates a separate interface aspect handling which are coupled with the InterfaceLayerRelationship stereotyped relationship. This is to avoid excessive port nesting for more complex interfaces (Tower of Hanoi / Towers of Bramha syndrome).
* Create the interfaces of the Physical System as they are existing in real-world (as-build) - as-planned is scope of the Functional Domain.
* In Physical Domain all proxyPorts have to be classified by an SAF_PhysicalInterfaceDefinition.

[>>> back to cheat sheet overview](../CheatSheet.md)
