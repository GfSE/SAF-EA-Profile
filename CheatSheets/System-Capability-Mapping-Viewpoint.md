# SFV08a System Capability Mapping VP

## Purpose
The System Capability Mapping Viewpoint describes the relationships of System Capabilities. The reasoning for System Capabilities as support for System Use Cases and the contribution of System Processes to Capabilities are described. Furthermore, the mapping of System Capabilities to Operational Capabilities are identified.

## Example

## Workflow
**Viewpoint Input:**
* SAF_SystemCapability from [SFV02b](System-Capability-Viewpoint.md)
* SAF_OperationalCapability from [SOV02c](Operational-Capability-Viewpoint.md)
* SAF_SystemRequirement from [SFV06a](System-Requirement-Viewpoint.md)
* SAF_SystemFunction and SAF_SystemProcess from [SFV02c](System-Process-Viewpoint.md)
* SAF_SystemUseCase from [SFV01a](System-Use-Case-Viewpoint.md)

**Step-by-Step Guide:**
1.	If needed, create an System Capability Mapping diagram as specialized [SysML 1.5 Block Definition Diagram](https://sparxsystems.com/enterprise_architect_user_guide/16.1/modeling_languages/block_definition_diagrams.html) with Add Diagram > SAF > BlockDefinition > SAF_SFV08a_SystemCapabilityMappingView.
2.	Create (and maintain) a matrix specification to link System Capability to Operational Capability by using the SAF_SystemCapabilityEnabling stereotype. Set the link accordingly.
3.	Create (and maintain) a matrix specification to link System Requirements to System Capability by using the SAF_SystemRequirementRefinement stereotype. Set the link accordingly.
4.	Create (and maintain) a matrix specification to link System Function to System Capability by using the System Function Enabling stereotype. Set the links accordingly.
5.	Create (and maintain) a matrix specification to link System Process to System Capability by using the System Process Enabling stereotype. Set the links accordingly.
6.	Create (and maintain) a matrix specification to link System Capability to System Use Cases by using the System Capability Support. Set the dependency links accordingly.
7.	Use the SAF standard search for the current traceability/mapping report by pressing Ctrl+F > SAF > SFV08b_SystemCapabilityMapping. 

**Viewpoint Output:**
* External: Traceability supports the quality control of the model, showing “lose ends” or inconsistencies. Also, it supports impact analyses for change management and assessments.

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* [SAF_SystemCapability](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_SystemCapability)
* [SAF_SystemCapabilitySupport](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_SystemCapabilitySupport)
* [SAF_SystemFunctionSupport](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_SystemFunctionSupport)
* [SAF_SystemFunction](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_SystemFunction)
* [SAF_SystemProcessEnabling](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_SystemProcessEnabling)
* [SAF_SystemProcess](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_SystemProcess)
* [SAF_SystemRequirement](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_SystemRequirement)
* [SAF_SystemUseCase](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_SystemUseCase)
* 
## General Recommendations and Pitfalls
* When deriving System Capabilities from Operational Capabilities, it has to be ensured that the System Capabilities fit to the System of Interest definition. Also, System Capabilities should fit to the defined System Stories. Both these relations are not documented in any viewpoint but have to be respected to ensure a consistent definition of the System of Interest.

[>>> back to cheat sheet overview](../CheatSheet.md)
