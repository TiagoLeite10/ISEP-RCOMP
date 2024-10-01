RCOMP 2022-2023 Project - Sprint 2 planning
===========================================
### Sprint master: 1211304 ###

# 1. Sprint's backlog #

| Task  | Task description                                                                                                                                                                                       |
|-------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| T.1.1 | Development of a layer two and layer three Packet Tracer simulation for building A, encompassing the campus backbone. Integration of every member’s Packet Tracer simulation into a single simulation. |
| T.1.2 | Development of a layer two and layer three Packet Tracer simulation for building B, encompassing the campus backbone.                                                                                  |
| T.1.3 | Development of a layer two and layer three Packet Tracer simulation for building C, encompassing the campus backbone.                                                                                  |
| T.1.4 | Development of a layer two and layer three Packet Tracer simulation for building D, encompassing the campus backbone.                                                                                  |
| T.1.5 | Development of a layer two and layer three Packet Tracer simulation for building E, encompassing the campus backbone.                                                                                  |


# 2. Technical decisions and coordination #
* **Packet Tracer Version:** V 8.2.0

## Conventions

* The name of the complete file should be campus.pkt;
* There should be a file for each building;
* Each building file should be named "buildingX.pkt", where X means the letter of the building;

#### Devices naming

* **Routers:** [R][Router Number]_Building Number (Example: R3_A)
* **Switches:** [Cross Connect Type][Switch Number]_Building Number (Example: CP1_A)
* **PCs or Laptops:** PC|Laptop Number_Building Number (Example: PC1_A)
* **Wireless Access Points:** WAP Number_Building Number (Example: WAP1_A)
* **IP-phones:** IPphone number_Building Number (Example: ipPhone1_A)

## VTP domain name

* rc23dig3

#### VLAN database
* **Range of VLAN IDs used:** 550 - 580

| Building     | Vlan Id Range |
|--------------|---------------|
| A + Backbone | 550 - 555     |
| B            | 556 - 560	    |
| C            | 561 - 565	    |
| D            | 566 - 570	    |
| E            | 571 - 575	    |

| Vlan Id | VLAN name    |
|---------|--------------|
| 550     | backbone     |
| 551     | Agroundfloor |
| 552     | Afloorone    |
| 553     | Awifi        |
| 554     | Admz         |
| 555     | Avoip        |
| 556     | Bgroundfloor |
| 557     | Bfloorone    |
| 558     | Bwifi        |
| 559     | Bdmz         |
| 560     | Bvoip        |
| 561     | Cgroundfloor |
| 562     | Cfloorone    |
| 563     | Cwifi        |
| 564     | Cdmz         |
| 565     | Cvoip        |
| 566     | Dgroundfloor |
| 567     | Dfloorone    |
| 568     | Dwifi        |
| 569     | Ddmz         |
| 570     | Dvoip        |
| 571     | Egroundfloor |
| 572     | Efloorone    |
| 573     | Ewifi        |
| 574     | Edmz         |
| 575     | Evoip        |

#### IPv4 network

| Building | Nodes | IPv4 Networks  |
|----------|-------|----------------|
| A        | 335   | 10.81.144.0/23 |
| E        | 220   | 10.81.146.0/23 |
| B        | 218   | 10.81.148.0/24 |
| C        | 190   | 10.81.149.0/24 |
| D        | 188   | 10.81.150.0/24 |
| Backbone | 100   | 10.81.151.0/25 |

####  ISP router IPv4 node address

* 121.60.202.181/30


# 3. Subtasks assignment #

  * 1211304 - T.1.1
  * 1191369 - T.1.2
  * 1211314 - T.1.3
  * 1210805 - T.1.4
  * 1191296 - T.1.5
