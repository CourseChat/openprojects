
# Extending telemetry to comprehensive site digital twin
> [!info] Digital Twin meets Zero Trust
> 
> This is an overview of an XIO **Digital Twin** initiative to offer a new service to existing and prospective customers: build an executable real-time model of their system and all of its components, with a new, inherent capability to sense intrusions, code insertions, and PLC signal path alterations. From this, create a specific plan for migration to a Zero-Trust architecture, component by component. Here are the steps to take with an existing customer.


## Start with sensor list
- Map all existing sensor and actuator feeds to XiO cloud
- List all potential sensor and actuator feeds
- Create AWWA template for example facilities, listing example configurations
	- Pipes, pumps, valves, tanks, reservoirs,
	- All SCADA elements
	- All PLCs
	- All racks, monitoring computational elements, interconnection plug boards, routers
	- All signal transmission paths
## Add all system documents: design, build, installation, maintenance 
> [!info] Build the system history repository
> 
> This is a new function and new expense for XIO. Essentially, add a small archivist and librarian staff for documentation, cataloging, OCR, and ingestion.  See "Semantic Scholar". This systematizes the XIO customer relationship, and is an inducement service for new customers, who may be overwhelmed by the challenges of moving to a machine learning environment.

- Create a complete picture of all system elements: how they interact, how they were installed and maintained, add all vendor information: purchase date, warranties, service contracts, hardware and software updates and repairs
- Inventory all documentation; annotate each document with file type, creation date, modification date, owner, editor, viewer identification; use template for creation of Zero Trust architecture
- Include Working drawings of system and system elements: 
	- scan, digitize, OCR original system records
	- include all field documents with any installation comments
		- final as-built documentation and drawings
		- transmission standard; interconnect location, maintenance and inspection records
- Spreadsheets detailing operations: projected flows, pressures, power demands
- Component manuals
- Installation records
- Certification of installation records
- Maintenance records
## Create System Repository (SR) or archive for each customer
> [!info] Use new LLM tools to vectorize all elements in the System Repository
> 
> Combine with existing LLM to generate graphs of existing system elements and their interrelationships, then use Google Notebook to generate Jupyter Notebooks for the overall system, and for each component. As the JN execute, they build the graphical representation of flows, power usage, pipe and pump operating state: vibration, temperature, strain, pipe wall thickness, amperage. Add in Distributed Fiber Optic sensing, soil chemistry.

## Build  an executable XIO Template (ET) for each customer 
> [!info] Here is the Jupyter Notebook built in 2018 to capture XIO data. It downloads 525,600 rows of data a year: one reading a minute. This is discrete enough for operational alerts for system managers.
> 
>  (https://colab.research.google.com/drive/1XcQYlQx4mYPJjRZNO0gxnHKXhaJhBEgG#scrollTo=S6FGOF65K6Gd)

It was complicated to get the XiO token to allow the download from AWS.  Need to redo this with today's archived Kibera Town Centre data at AWS.

[Getting XiO data for 2 years](https://colab.research.google.com/drive/1XcQYlQx4mYPJjRZNO0gxnHKXhaJhBEgG#scrollTo=S6FGOF65K6Gd)

[Getting a smaller data amount from 2018 due to broken XiO security certificate](https://colab.research.google.com/drive/1a0pWsx7NApO7P4rfiIl0MuBlhlezAcha#scrollTo=0OmzkMqwFsOt)

[A third Colab JN]([https://colab.research.google.com/drive/1a0pWsx7NApO7P4rfiIl0MuBlhlezAcha#scrollTo=-QN715QW3ces](https://colab.research.google.com/drive/1a0pWsx7NApO7P4rfiIl0MuBlhlezAcha#scrollTo=-QN715QW3ces))
14:04 2024-11-25
[This Colab actually gets a token from XiO](https://colab.research.google.com/drive/1a0pWsx7NApO7P4rfiIl0MuBlhlezAcha#scrollTo=O204TtGngozK)





> [!tip] Use Brick ontology for system descriptions
> 
> As XiO builds a set of example systems, a main goal is to create an AWWA standard system description that can be adopted by the AWWA Technical Innovations committee, chaired by Clifford Chan, CEO of EBMUD. 
> For national or international adoption as a standard, major player must be convinced of the value and legitimacy of the new LLM work plan. [[Brick]], from UC Berkeley and Colorado School of Mines, can be a framework.
> 
> see [[Work Plan]]

- For overall system; for each component; for each data source and sink 
- Use Google Notebook to create this template from the System Repository
- Create executable Jupyter Notebook (JN) for each component, capturing all data flows
- Create JN for overall system
	- Think of this as a real-time spreadsheet for an operational system
	- Think of each component as an executable object
- See Work Plan Examples showing running Jupyter Notebooks at  Colab
## Use this ET to validate **Zero Trust Implementation**
- Build analyzer showing user authentication, component authentication, roles, authorities
- Build customer roadmap for replacement of archaic Microsoft OS, applications
	- Utilize new Microsoft commitment to Zero Trust
- Original XIO Real Time telemetry
[Link to Real Time Telemetry](https://johngage.github.io/XIO-OperationalDataKTC/)

## [[Work Plan Examples]]
> [!info] Using XIO historical customer data from five years of **Kibera Town Centre** operation
> 
> Here is an example of a Jupyter Notebook for the Waste Water system at KTC, built by ingesting a GoogleDocs spreadsheet of all system components, visible below. Using Anthropic **Claude** as the LLM, this document was ingested, and from the diagram,  created a list of all components and their position in the flow. From that, **Claude** created Jupyter Notebooks. ** Google Notebook** created a variant. The **JN** then was copied to **Google Colabs**, where it is running now, with Python pseudo-code calculating system power, system pressure and system flows, tank capacity and tank flows......ready to be elaborated with as detailed hydrology as desired, and as elaborate time-series analysis as desired.

- [Resulting Jupyter Notebook at Colab](https://colab.research.google.com/drive/1T6J97EZrM3TwkW_A9YDfJUA3p8SjnB2Y#scrollTo=EcZjG90NVENZ)
- See Google Notebook
- [[Water Organizations]] **Potential Test Site Partners**

## XIO  Real-Time Telemetry Examples
### Build examples of **existing site designs** extended to digital twins
	- All Stanford existing telemetry projects
		- Storm water monitoring
		- Reservoir levels: use this weekend Atmospheric River monitoring records
		- Warm water temperature capture from dormitories
		- Flows; energy use; 
	- Kibera Town Centre
	- Ventura County
	- Russian River
	- Existing customers who have given permission to use in XiO demonstrations
- ### Add new telemetry customers
	- Add **Palo Alto** as a partner, since they own power, water, sewage, telecom
	- Add **UC Berkeley Center for Smart Infrastructure**
	- Add **UC Berkeley Campus projects for geothermal building heating and cooling**
	- Add **Google new building**
### Advanced Metering Infrastructure installations
	- Amazon 
	- [CivilGrid](https://www.civilgrid.com/#home-partners)
	- New telemetry connections for schools, public facilities
	- Flume
	- Flo
	- Oracle, Sensus, Badger, AquaMetric, 
## Incorporate conversion to [[Zero-Trust Environment]]
	- Operating-system dependent
		- SCADA sites overwhelmingly use insecure and outdated Microsoft software
		- Use new Microsoft commitment to [[Zero-Trust Environment]]; 
		- partner with Amazon in establishing metering RF infrastructure for water utilities
			- 
	- Move to post-SCADA security
	- Incorporate machine-learning models for system maintenance and rebuild models
	- Re-engineer emergency response systems for advanced pipe, pump and valve replacement schedule

---
### Stanford University

- Existing customer installation
- Campus-wide integration of sensor data feeding into system modeling
- Use model as an extension to Stanford curriculum; annotate use by research elements

---

### UC Berkeley
- [Center for Smart Infrastructure](https://geotechnical.berkeley.edu/sites/default/files/CSI%20Overview.pdf)
- [UC Berkeley Center for Smart Infrastructure](https://smartinfrastructure.berkeley.edu/)
- 
### California Rural Water Association
- [4,000 members](https://www.officialmediaguide.com/crwa/)
- Add [CWEA wastewater](https://www.cwea.org/) 
- [Training and standards](https://calruralwater.org/)
- [National Rural Water Association](https://nrwa.org/rural-water-rally/)
- 
### Kibera Town Centre: Nairobi, Kenya

![XIO 2018](https://docs.google.com/spreadsheets/d/1vzGa6wepsXOBiFh2k5qptadJ4B0HjZh3NEVsS7CHkcs/edit?pli=1&gid=0#gid=0)
### To be added
- [Balance Hydrologics](https://xiowatersystems-my.sharepoint.com/:b:/g/personal/colinb_xiowatersystems_onmicrosoft_com/EX6ot7QvyYpAmhNy-VITfpAB5ERIYYjk4Y6ihUCBwQvCWQ?e=aXc1Qx) - Build vs. Buy a Cloud Platform
- [Cobb Area Water District](https://xiowatersystems-my.sharepoint.com/:b:/g/personal/colinb_xiowatersystems_onmicrosoft_com/EczsGWCOWEpAkuj-EymxuCABKw-JSg0CzTdFZHzGKD2ZAQ?e=Ipaddi) - State Consolidation made Easy
- [Cold Springs Water Company](https://xiowatersystems-my.sharepoint.com/:b:/g/personal/colinb_xiowatersystems_onmicrosoft_com/EZJZCGvB78VCn2tTWmuluWcBr-ZqWUosXRpAbu7Ta-gB5A?e=lTPWT7) - Continued Management despite Record Snowfall
- [Russian River Utility - Distributed Managed Operations](https://xiowatersystems-my.sharepoint.com/:b:/g/personal/colinb_xiowatersystems_onmicrosoft_com/ETPyNxf121NAmnIahq5STAMBLP2liLWopBuwn4sgM3m8-w?e=hHyZjV) - Boost efficiency, reduce operations costs
- [Pleasant Valley Water District - Energy, Water, and Cost Savings](https://xiowatersystems-my.sharepoint.com/:b:/g/personal/colinb_xiowatersystems_onmicrosoft_com/EcPHCeV3169LjdNo7yQfwxgBnk6-B0My05D8ToXaZiKQ7Q?e=jQ5mAZ) - Cloud Computing optimizes energy usage


---

<iframe src="https://docs.google.com/spreadsheets/d/1vzGa6wepsXOBiFh2k5qptadJ4B0HjZh3NEVsS7CHkcs/edit?pli=1&gid=0#gid=0"></iframe>

---

Link to docs.google.com/spreadsheets

[Link to XIO sensor detail 2018](https://docs.google.com/spreadsheets/d/1vzGa6wepsXOBiFh2k5qptadJ4B0HjZh3NEVsS7CHkcs/edit?pli=1&gid=0#gid=0)

---

iframe from docs.google.com/spreadsheets
<iframe src="https://docs.google.com/spreadsheets/d/1vzGa6wepsXOBiFh2k5qptadJ4B0HjZh3NEVsS7CHkcs/edit?pli=1&gid=0#gid=0" width="1000px" height="3000px"></iframe>


---

## XIO customer base: 1000 accounts
### Stanford
### Florida
### CRLA
### AWWA

---


- 