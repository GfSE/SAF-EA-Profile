# SPV08b Physical Functional Mapping VP

## Purpose
The Physical Functional Mapping Viewpoint supports the analysis of the assignment (it is derived relationship) of system functions and system partial functions to physical SOI elements.

## Example

## Workflow
**Viewpoint Input:**
* Functional to Logical Mapping from [SLV08a](Logical-Functional-Mapping-Viewpoint.md)
* Logical to Physical Mapping from [SPV08a](Physical-Logical-Mapping-Viewpoint.md)

**Step-by-Step Guide:**
1.	Use the SAF standard search for the current mapping report by pressing Ctrl+F > SAF > SPV08b_PhysicalFunctionalMapping_Context and/or SLV08a_PhysicalFunctionalMapping_Internal.	

**Viewpoint Output:**
* External: Traceability supports the quality control of the model, showing “lose ends” or inconsistencies. Also, it supports impact analyses for change management and assessments.

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* Allocate
* [SAF Function Action](https://saf.gfse.org/userdoc/stereotypes.html#saf_functionaction)
* [SAF_LogicalContextRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_logicalcontextrole)
* [SAF_PhysicalContextRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalcontextrole)
* [SAF_LogicalInternalRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_logicalinternalrole)
* [SAF_PhysicalInternalRole](https://saf.gfse.org/userdoc/stereotypes.html#saf_physicalinternalrole)
  
## General Recommendations and Pitfalls
* This viewpoint summerizes the mapping from Functional to Logical to Physical items. In case the mapping/traceability has a gap the specific traceability steps in [SLV08a](Logical-Functional-Mapping-Viewpoint.md) and [SPV08a](Physical-Logical-Mapping-Viewpoint.md) have to be checked.

[>>> back to cheat sheet overview](../CheatSheet.md)
