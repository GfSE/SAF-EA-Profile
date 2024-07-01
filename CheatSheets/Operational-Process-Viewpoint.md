# SOV03a Operational Process VP

## Purpose
The Operational Process Viewpoint describes the Operational Processes related to a specific Operational Story, the sequence of execution, and their Operational Exchanges, including information, materials, natural resources, etc. The assignment of Operational Processes to Operational Performers is captured.

## Example

## Workflow
Viewpoint Input:
* Operational Story from SOV01a which need a refinement
* Operational Roles from SOV01b which perform actions.
* Operational Domain Item Kinds as object flows between the actions.

Step-by-Step Guide:
1.	Create an Operational Process item in the dedicated package in your model to formalize an Operational Story or to expose a scenario.
2.	Create a new SAF Operational Process diagram for the new Operational Process - right-click on the Operational Process, select New Child Diagram > Add Diagram > SAF > Activity > SAF::SOV03a_OperationalProcessView.
3.	Drag and drop an involved Operational Performer onto the diagram and create an Operational Role by selecting partition in the dialog
4.	Add Operational Process Actions to the according partition by drag and drop of existing Operational Processes and selecting instance.
5.	For new Operational Process Actions create an Operational Process in the dedicated package with Add Element > Toolset: All Perspectives / SAF > Type: Operational Process. Proceed with step 4.
6.	Model control and object flows by using the Quick Linker. For object flows you can set the information flow from the object flow’s context menu with Advanced > Information Flows Realized. Click on the empty field to browse or search for the Operational Domain Kind that has been created previously.

Viewpoint Output:
* Stakeholder Requirements (SOV06a) can be elicit from the processes.

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* [SAF_OperationalContextRole](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalContextRole)
* [SAF_OperationalDomainKind](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalDomainKind)
* [SAF_OperationalPerformer](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalPerformer)
* [SAF_OperationalProcessAction](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalProcessAction)
* [SAF_OperationalProcess](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalProcess)

For other notation elements which are exposed in the viewpoint, consider UML/SysML standard reference literature.

## General Recommendations and Pitfalls
* Due to tool restrictions, the Operational Process Actions are not automatically allocated to Operational Roles by assigning them to partitions in the diagram. Therefore, it is mandatory to maintain the allocation matrix as per SAF SOV08a Operational Process Traceability Viewpoint.
* Operational Process Actions have to be broken down until they can be unambiguously assigned to single Operational Roles.
* If the focus of the modeling activity is to describe the interaction between the different performers and not on the flow of activities, it is recommended to use an Operational Interaction diagram instead.
* A consistency between Operational Processes and Operational Capabilities has to be ensured if both are defined in a project.
