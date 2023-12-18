# Sparx Systems Enterprise Architect Repository, TdSE2023 Release
The repository features the EA SAF Profile as MDG Technology with supplemental material. The SAF profile is intended to be used with EA 16 and EA’s SysML1.5 MDG.

# safMDG.xml
System Architecture Framework Profile has been created by the SAF Working Group of the German Chapter of INCOSE (GfSE). The SAF Profile provides the stereotypes, specification views and linking rules according to the [SAF-Specification](https://github.com/GfSE/SAF-Specification/tree/TdSE2023) based on EA's MDG Technology.

# How to use safMDG
Download the safMDG.xml, import and activate the MDG by considering the following [step-by-stype guide](https://sparxsystems.com/enterprise_architect_user_guide/16.0/modeling_frameworks/access_remote_mdg_technologies.html).

![Enable the SAF Profile](/pics/mdg.png)

# How to establish a view based on a SAF Viewpoint
SAF Viewpoints are realised by EA view specifications based on SysML. Therefore, the view can be established easily by creating a diagram, select SAF, the according SysML base diagram and select the demanded view specification e.g. Activity >>> SAF::SFV03a_SystemProcessView. Within the view specification which applies to a diagram all relevant SAF stereotypes are available and the particular viewpoint linking rules apply.

![Apply a VP](/pics/view_spec.png)

# How to use the SQL Queries
The SAF profile contains multiple queries helping to manage your traceability in your model (SxV08 aspect Mapping). Please note that all queries are developed for qea files / DBMS. The queries do not work for local eap(x) files (JET 4 Engine).
Basically the queries are available in Searches -> Search Category "SAF". As the query itself is editable it can be copied into a model view within any SxV08 view.

The following queries are available:
* **SOV08a_OperationalCapabilityMapping** - depicts any Operational Story, Operational Performer or Stakeholder Requirement if linked to the Operational Capability
* **SOV08b_OperationalProcessMapping** - depicts any Operational Story, Operational Story if linked to the Operational Process. Furthermore the query derives any Operational Performer which are exhibited as AcitivityPartition in an Operational Process View.
* **SFV08a_SystemCapabilityMapping** - depicts any System Use Case, Operational Capability, System Process or System Requirement if linked to the System Capability
* **SFV08b_SystemRequirementTraceability** - lists the source of System Requirements, if linked. Furthermore the query lists also all System Requirements which have not a source linked.
* **SLV08a_LogicalFunctionalMapping_Context** - derives allocations between black-box (System Functions or Context Functions) to (Logical SOI, Logical External System, Logical Environment or Logical User), based on allocation or partitions (call behavior within activity partitions) among instances. The query considers elements without a link as well.
* **SLV08a_LogicalFunctionalMapping_Internal** - derives allocations between white-box System Partial Functions to Logical Elements, based on allocation or partitions (call behavior within activity partitions) among instances. The query considers elements without a link as well.
* **SPV08a_PhysicalLogicalMapping_Context** - derives allocations between black-box (Logical SOI, Logical External System, Logical Environment or Logical User) to (Phyiscal System, Physical External System, Physical Environment or Physical User), based on allocation among instances. The query considers elements without a link as well.
* **SPV08a_PhysicalLogicalMapping_Internal** -  derives allocations between white-box Logical Elements to (Phyiscal Elements, Physical Software Elements or Physical Hardware Elements), based on allocation among instances. The query considers elements without a link as well.
* **SPV08b_PhysicalFunctionalMapping_Context** - derives 2-step allocations between black-box (System Functions or Context Functions) to (Phyiscal System, Physical External System, Physical Environment or Physical User) via (Logical SOI, Logical External System, Logical Environment or Logical User), based on allocation or partitions (call behavior within activity partitions) among instances. The query considers elements without a link as well.
* **SPV08b_PhysicalFunctionalMapping_Internal** - derives 2-step allocations between white-box System Partial Functions to (Phyiscal Elements, Physical Software Elements or Physical Hardware Elements) via Logical Elements, based on allocation or partitions (call behavior within activity partitions) among instances. The query considers elements without a link as well.

![SQL Query](/pics/queries.png)
