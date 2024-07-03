# SLV02a Logical Internal Interaction VP

## Purpose
The Logical Internal Interaction Viewpoint describes System internal behavior based on the exchange between the Logical SOI Elements Usage. It depicts the sequence of interactions between the Logical SOI Elements and the exchanged Domain Item Kinds needed to accomplish a System Partial Function.

## Example

## Workflow
**Viewpoint Input:**
* SAF_SystemFunction from [SFV02c](System-Functional-Breakdown-Viewpoint.md) which needs refinement
* SAF_LogicalInternalRole from [SLV02a](Logical-Structure-Definition-Viewpoint.md)
* itemFlows from [SLV04c](Logical-Internal-Exchange-Viewpoint.md)
* SAF_DomainItemKind as exchange items between Logical Internal Roles from [SFV02a](System-Domain-Item-Kind-Viewpoint.md)

**Step-by-Step Guide:**
1.	Select a System Function item in the dedicated package in your model to formalize a System Function and create a new SAF Logical Internal Interaction diagram as specialized [SysML 1.5 Sequence Diagram](https://sparxsystems.com/enterprise_architect_user_guide/16.1/modeling_languages/sysml-seq-diagram.html) for the System Function - right-click on the System Function, select Add > Add Diagram > SAF > Sequence > SAF::SLV04a_LogicalInteractionView.
3.	Drag and drop Logical Internal Roles onto the diagram which are involved in the interaction.
4.	Define the sequence in the interaction with messages.
5.	Select the message > right-click on the Connector > Advanced > Information Flow Realized > Select the available Operational Domain Kind(s).

**Viewpoint Output:**
* new defined itemFlows back to [SLV04c](Logical-Internal-Exchange-Viewpoint.md)

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* Interaction
* Lifeline
* Message
* [SAF_LogicalInternalRole](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_LogicalInternalRole)

## General Recommendations and Pitfalls
* It is required that the exchanges in [SLV04b](Logical-Internal-Exchange-Viewpoint.md) are addressed in this diagram to ensure consistency.

[>>> back to cheat sheet overview](../CheatSheet.md)
