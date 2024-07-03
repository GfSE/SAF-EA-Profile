# SPV02a Physical Structure Definition VP

## Purpose
The Physical Structure Viewpoint is used to model the internal structure of the SOI and to identify the internal system elements making up the SOI. The SOI breakdown structure identifies system elements and finally at the implementation level hardware, software, and mechanics. The SOI breakdown structure determines items that are reused and make-or-buy (COTS) items. The Physical Structure Viewpoint is elaborated for each candidate physical SOI architecture. It provides the basis for further assessment of the architecture candidates by identifying the system elements in each candidate solution.

## Example

## Workflow
**Viewpoint Input:**
* the SAF_PhysicalSystem from [SPV01b](Physical-Context-Definition-Viewpoint.md)

**Step-by-Step Guide:**
1.  Create a new Logical Structure Definition diagram as specialized [SysML1.5 Block Definition Diagram](https://sparxsystems.com/enterprise_architect_user_guide/16.1/modeling_languages/block_definition_diagrams.html) in the dedicated package in your model with Add Diagram > SAF > BlockDefinition > SAF::SPV02a_PhysicalStructureView.
2. Drag and drop your Physical System to the diagram.
3. Create Physical Elements which represent parts of your system.
4. Create Physical Internal Roles by using the composition relationship. Give the Physical Internal Role a meaningful name by selecting the part property in the Physical System and amending the name on the property element page for traceability purposes in matrix specifications.
5. If needed, define the multiplicity for the Physical Internal Roles.

**Viewpoint Output:**
* SAF_PhysicalInternalRoles which are used in [SPV04b](Physical-Internal-Exchange-Viewpoint.md)
* SAF_LogicalInternalRoles are allocated to SAF_PhysicalInternalRoles in [SPV08a](Physical-Logical-Mapping-Viewpoint.md)

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* [SAF_PhysicalElement](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_PhysicalElement)
* [SAF_PhysicalHardwareElement](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_PhysicalHardwareElement)
* [SAF_PhysicalSoftwareElement](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_PhysicalSoftwareElement)
* [SAF_PhysicalSystem](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_PhysicalSystem)

## General Recommendations and Pitfalls
* Name the properties as for traceability management in Enterprise Architect the matrix specification displays the element name only.
* The physical structure of the SOI represents the building plan as the physical elements represent material parts with part number, manufacturer code etc. The breakdown structure is often standardized within an organization.
* Please note that the breakdown might consist of appropriate material parts, but also additional elements for structural arrangement purposes only ("Auxillary"). These elements (without a life-cycle) represent only a collection of appropriate structural elements. It is recommended to mark the elements (e.g. with tagged value). 

[>>> back to cheat sheet overview](../CheatSheet.md)
