# Sparx Systems Enterprise Architect Repository
The repository features the EA SAF Profile as MDG Technology with supplemental material. The SAF profile is intended to be used with EA 16 and EA’s SysML1.5 MDG.

# safMDG.xml
System Architecture Framework Profile has been created by the SAF Working Group of the German Chapter of INCOSE (GfSE). The SAF Profile provides the stereotypes, specification views and linking rules according to the [SAF-Specification](https://saf.gfse.org) based on EA's MDG Technology.

# How to use safMDG
Download the safMDG.zip by [entering the zip-file](https://github.com/GfSE/SAF-EA-Profile/blob/main/safMDG.zip) in the list and select the download button (Download raw file).
Extract the XML, import and activate the MDG by considering the following [step-by-stype guide](https://sparxsystems.com/enterprise_architect_user_guide/16.0/modeling_frameworks/access_remote_mdg_technologies.html).

![Enable the SAF Profile](/pics/mdg.png)

# How to establish a view based on a SAF Viewpoint
SAF Viewpoints are realised by EA view specifications based on SysML. Therefore, the view can be established easily by creating a diagram, select SAF, the according SysML base diagram and select the demanded view specification e.g. Activity >>> SAF::F3_SFRE_View. Within the view specification which applies to a diagram all relevant SAF stereotypes are available and the particular viewpoint linking rules apply.

![Apply a VP](/pics/view_spec.png)

# How to use the SQL Queries
The SAF profile contains multiple queries helping to manage your traceability in your model. Please note that all queries are developed for qea files / DBMS. The queries do not work for local eap(x) files (JET 4 Engine).
Basically the queries are available in Searches -> Search Category "SAF". As the query itself is editable it can be copied into a model view within any diagram.

The following queries are available:
The following queries are available:
* **O8_OCYM Operational Capability Mapping** - depicts any Operational Story, Operational Performer or Stakeholder Requirement if linked to the Operational Capability
* **O8_OPRM Operational Process Mapping** - depicts any Operational Story, Operational Story if linked to the Operational Process. Furthermore the query derives any Operational Performer which are exhibited as AcitivityPartition in an Operational Process View.
* **F8_SCYM System Capability Mapping** - depicts any System Use Case, Operational Capability, System Process or System Requirement if linked to the System Capability
* **F8_SRQT System Requirement Traceability** - lists the source of System Requirements, if linked. Furthermore the query lists also all System Requirements which have not a source linked.
* **L8_LFUM Logical Functional Mapping - Context** - derives allocations between black-box (System Functions or Context Functions) to (Logical SOI, Logical External System, Logical Environment or Logical User), based on allocation or partitions (call behavior within activity partitions) among instances. The query considers elements without a link as well.
* **L8_LFUM Logical Functional Mapping - Internal** - derives allocations between white-box System Partial Functions to Logical Elements, based on allocation or partitions (call behavior within activity partitions) among instances. The query considers elements without a link as well.
* **P8_PLOM Physical Logical Mapping - Context** - derives allocations between black-box (Logical SOI, Logical External System, Logical Environment or Logical User) to (Phyiscal System, Physical External System, Physical Environment or Physical User), based on allocation among instances. The query considers elements without a link as well.
* **P8_PLOM Physical Logical Mapping - Internal** -  derives allocations between white-box Logical Elements to (Phyiscal Elements, Physical Software Elements or Physical Hardware Elements), based on allocation among instances. The query considers elements without a link as well.
* **P8_PFUM Physical Functional Mapping - Context** - derives 2-step allocations between black-box (System Functions or Context Functions) to (Phyiscal System, Physical External System, Physical Environment or Physical User) via (Logical SOI, Logical External System, Logical Environment or Logical User), based on allocation or partitions (call behavior within activity partitions) among instances. The query considers elements without a link as well.
* **P8_PFUM Physical Functional Mapping - Internal** - derives 2-step allocations between white-box System Partial Functions to (Phyiscal Elements, Physical Software Elements or Physical Hardware Elements) via Logical Elements, based on allocation or partitions (call behavior within activity partitions) among instances. The query considers elements without a link as well.

![SQL Query](/pics/queries.png)

## Versions
This is the main branch, reflecting the current development and it is updated as appropriate.

The following releases are available, each is kept in a separate branch:
* [Initial Release](https://github.com/GfSE/SAF-EA-Profile/tree/Initial-Release)
* [TdSE2022](https://github.com/GfSE/SAF-EA-Profile/tree/TdSE2022)
* [TdSE2023](https://github.com/GfSE/SAF-EA-Profile/tree/TdSE2023)
* [TdSE2024](https://github.com/GfSE/SAF-EA-Profile/tree/TdSE2024)
* [TdSE2025](https://github.com/GfSE/SAF-EA-Profile/tree/TdSE2025)
