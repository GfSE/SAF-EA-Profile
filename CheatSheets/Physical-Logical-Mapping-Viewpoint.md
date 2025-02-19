# SPV08a Physical Logical Mapping VP

## Purpose
The Physical Logical Mapping Viewpoint supports the definition of the assignment of conceptual logical system elements to physical SOI elements.
Following the identification of physical SOI elements capable of performing the system functions of logical elements, the Physical Logical Mapping Viewpoint provides feedback to the System Architecture Definition process to consolidate or confirm the allocation, partitioning, and alignment of logical elements to physical elements that comprise the SOI.

## Example

## Workflow
**Viewpoint Input:**
* SAF_LogicalContextRole from [SFV01b](System-Definition-Viewpoint.md)
* SAF_LogicalInternalRole from [SLV02a](Logical-Structure-Definition-Viewpoint.md)
* SAF_PhysicalContextRome from [SPV01b](Physical-Definition-Viewpoint.md)
* SAF_PhysicalInternalRole from [SPV2a](Physical-Structure-Definition-Viewpoint.md) 

**Step-by-Step Guide:**
1.  Create an Physical Logical Mapping diagram as specialized [SysML 1.5 Block Definition Diagram](https://sparxsystems.com/enterprise_architect_user_guide/16.1/modeling_languages/block_definition_diagrams.html) with Add Diagram > SAF > BlockDefinition > SAF::SPV08a_PhysicalLogicalMappingView.
2. 	Create (and maintain) a matrix specification to allocate Logical Context Roles to Physical Context Roles.
3.	Create (and maintain) another matrix specification to allocate Logical Internal Roles to Physical Internal Roles.
4.	Use the SAF standard search for the current mapping report by pressing Ctrl+F > SAF > SPV08a_PhysicalLogicalMapping_Context and/or SLV08a_PhysicalLogicalMapping_Internal.	

**Viewpoint Output:**
* External: Traceability supports the quality control of the model, showing “lose ends” or inconsistencies. Also, it supports impact analyses for change management and assessments.

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* Allocate
* [SAF_LogicalContextRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_logicalcontextrole)
* [SAF_PhysicalContextRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalcontextrole)
* [SAF_LogicalInternalRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_logicalinternalrole)
* [SAF_PhysicalInternalRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalinternalrole)

## General Recommendations and Pitfalls
* N/A

[>>> back to cheat sheet overview](../CheatSheet.md)
