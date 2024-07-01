# SOV01a Operational Performer VP

## Purpose
The Operational Performer Viewpoint represents the taxonomy of the identified Operational Performers, if existing and relevant for the understanding of the operation of the intended solution.

## Example

## Workflow
Viewpoint Input:
* N/A

Step-by-Step Guide:
1.	Create a new Operational Performer Diagram in the dedicated package in your model as specialized SysML1.5 Block Definition Diagram with Add Diagram > SAF > BlockDefinition > SAF::SOV02b_OperationalPerformerView.
2.	Drag and drop already identified Operational Performer or create new items on the diagram.
3.	If needed, you can establish an Operational Performer Composition relationship between two Operational Performer. Please note that the composition must be set from parent to child.
4.	Drag and drop already identified Operational Performer or create new Stakeholder on the diagram
5.	Link the Stakeholder(s) to the Operational Performer which it represents with the Operational Stakeholder Representation stereotype.

Viewpoint Output:
* Operational Performer are acting in operational stories (SOV01a), are part of an operational context (SOV01b) and are represented by stakeholder (SOV02d).

## Exposed Elements and Connectors
The following Stereotypes / Model Elements are used in the Viewpoint:
* [SAF_OperationalPerformer](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalPerformer)
* [SAF_OperationalPerformerComposition](https://github.com/GfSE/SAF-Specification/blob/TdSE2023/stereotypes.md#SAF_OperationalPerformerComposition)

## General Recommendations and Pitfalls
* If Operational Performers are added to the model while working on other viewpoints, they are not automatically added to the Operational Performer diagram. In such a case, they must be added manually (see workflow description).
* For better understanding for everyone involved in modeling, it is recommended to add descriptions to the Operational Performer “Text” attribute for each Operational Performer.
* For overview purposes the diagram can be displayed in specification view.
