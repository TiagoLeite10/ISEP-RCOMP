RCOMP 2021-2022 Project - Sprint 3 planning
===========================================
### Sprint master: 1211304 ###
(This file is to be created/edited by the sprint master only)

# 1. Sprint's backlog #
Considering the previous sprint, the team is now required continue working on the regarding building in order to adapt the static routing into a dynamic routing.
For this process, the OSPF will be the protocol used.

| Task | Task Description                                                                                                                                      |
|------|-------------------------------------------------------------------------------------------------------------------------------------------------------|
|T.3.1 | Update the campus.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building A. |
|T.3.2 | Update the campus.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building B. |
|      | Final integration of each member’s Packet Tracer simulation into a single simulation.                                                                 |
|T.3.3 | Update the campus.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building C. |
|T.3.4 | Update the campus.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building D. |
|T.3.5 | Update the campus.pkt layer three Packet Tracer simulation from the previous sprint, to include the described features in this sprint for building E. |

# 2. Technical decisions and coordination #
In this section, all technical decisions taken in the planning meeting should be mentioned. 		

-   All member used Cisco Packet Tracer version 8.2.0.

-   VTP domain name must be rc23dig3.

-   The main output is the Packet Tracer simulation file for the corresponding building, it should be named BuildingN.pkt, with N being the number which identifies the building.

-	The **OSPF area ids** are:
     - Backbone: 0
     - Building A: 1
     - Building B: 2
     - Building C: 3
     - Building D: 4
     - Building E: 5


-	The **VoIP prefixes** are:
     - Building A: 1...
     
     - Building B: 2...
     
     - Building C: 3...
     
     - Building D: 4...

     - Building E: 5...


-	The highest level DNS domain will be part of Building A, naming **rcomp-22-23-di-g3**.
     It will be used as if it was the DNS root domain.

-	The other DNS domains will be created locally in each building, naming **building-X.rcomp-22-23-di-g3**.
     The letter *X* will identify the building's number.

-	In each building, all DNS servers will have the unqualified DNA name as **ns**.
     While Building A will have **ns.rcomp-22-23-di-g3**, the others will have **ns.building-X.rcomp-22-23-di-g3**.

-	The **IPv4 node address** for each DNS name server are:
     - **Building A - ns.rcomp-22-23-di-g3**
          B1-DMZ: 10.81.144.128

	- **Building B - ns.building-B.rcomp-22-23-di-g3**
		B2-DMZ: 10.81.148.240
		
	- **Building C - ns.building-C.rcomp-22-23-di-g3**
		B3-DMZ: 10.81.149.224
		
	- **Building D - ns.building-D.rcomp-22-23-di-g3**
		B4-DMZ: 10.81.150.240
		
	- **Building E - ns.building-E.rcomp-22-23-di-g3**
		B5-DMZ: 10.81.147.32

# 3. Subtasks assignment #

  * 1211304 - T.1.1
  * 1191369 - T.1.2
  * 1211314 - T.1.3
  * 1210805 - T.1.4
  * 1191296 - T.1.5