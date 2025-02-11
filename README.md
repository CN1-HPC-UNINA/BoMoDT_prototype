# DIGITAL TWIN OF BOLOGNA: PROTOTYPE OF CN1-HPC-WP2 

BoMoDT is the **Mobility Digital Twin (MoDT)** platform specifically developed for the city of **Bologna (Bo)**, 
serving as an exemplary prototype that implements the CN1-HPC-WP2 Digital Twin reference architecture. 
BoMoDT is designed to deliver real-time monitoring, simulations, and optimization of the city's urban mobility 
infrastructure.

---

## **Table of Contents**

- [Overview](#overview)
- [High-Level Architecture](#high-level-architecture)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation Steps](#installation-steps)
- [System Requirements](#system-requirements)
- [References](#references)
- [License](#license)


## **Overview**

BoMoDT integrates traffic flow data streams from [**Bologna Open Data**](https://opendata.comune.bologna.it/) to 
create a dynamic and fidelity virtual representation of the city. The source code, the instruction for deploying the 
platform and execute the different use cases is available in 
[**this repository**](https://github.com/alessandrasomma28/BoMoDT). 

---
## **High-Level Architecture**

The high-level architecture of BoMoDT follows the design  defined by the **Digital Twin Reference Architecture** 
This architecture specifies the core building blocks and subsystems required for a fully operational Digital Twin. 
The domain independent and platform agnostic architecture, available in [**DTReferenceArchitecture repository**](https://github.com/CN1-HPC-UNINA/DTReferenceArchitecture), has been customized for the urban mobility scenario, 
considering two enabling technologies: 
- [**Eclipse Simulator of Urban MObility**](https://eclipse.dev/sumo/) (SUMO), an open-source, multi-modal, highly 
  portable traffic simulator, designed for simulating real-world traffic scenario.
- [**FIWARE**](https://www.fiware.org/), an open-source and standard based initiative that facilitates the development of smart solutions 
  such as Digital Twins.





## **Platform Capabilities**

- **Digital Representation and State Simulation:** Accurately models both the structural and behavioral aspects of 
  Bologna’s mobility infrastructure while simulating various traffic scenarios. BoMoDT utilizes the Eclipse SUMO tool 
  for comprehensive traffic modeling and  
  simulation.

- **Bidirectional Synchronization:** Facilitates seamless data flow between physical sensors and the Digital Twin 
  while allowing feedback from the Digital Twin to control real-world traffic light systems. BoMoDT employs FIWARE 
  Generic Enablers (GEs) to manage data exchange and ensure semantic interoperability between the physical 
  infrastructure and its Digital Twin.

- **Traffic Monitoring and Visualization:** 
  - A **Django WebApp** and a **Grafana dashboard** are used to:
    - *(i)* Monitor the status of context entities modeled using FIWARE Smart Data Models.
    - *(ii)* Track real-time traffic flow patterns via the Grafana Dashboard.
    - *(iii)* Visualize simulation outcomes after scenario completion.

  

