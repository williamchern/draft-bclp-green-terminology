---
title: "Terminology for Energy Efficiency Network Management"
abbrev: "Energy Efficiency Terminology"
category: info

docname: draft-bclp-green-terminology-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
area: "Operations and Management"
workgroup: "Getting Ready for Energy-Efficient Networking"
keyword:
 - Energy Efficient
 - Energy Saving
 - Energy Management

author:
 -
    fullname: Chunchi Liu
    organization: Huawei
    email: liuchunchi@huawei.com
 -
    fullname: Qin Wu
    organization: Huawei
    email: bill.wu@huawei.com
 -
    fullname: Mohamed Boucadair
    organization: Orange
    email: mohamed.boucadair@orange.com
 -
    fullname: Luis M. Contreras
    organization: Telefonica
    email: luismiguel.contrerasmurillo@telefonica.com
 -
    fullname: Marisol Palmero
    organization: Cisco
    email: mpalmero@cisco.com

normative:

informative:


--- abstract

Energy efficient network management involves deploying and managing network infrastructures to optimize energy
use on network devices while improving overall network utilization.

This document provides a glossary of terms used in the IETF when discussing energy efficiency Network management.
The purpose is to help frame discussions of energy efficiency in the various areas of the IETF and to help
introduce the main concepts to IETF participants.

--- middle

# Introduction

With rising energy costs and an increasing awareness of the ecological impact of running information technology
equipment, Energy efficiency has been seen to be a critical issue for network management systems in relation to
environmental impact and operational cost. Energy efficiency management functions and interfaces are becoming
an additional requirements for network management systems.

This document provides a glossary of terms used in the IETF when discussing energy efficiency Network management.
The purpose is to provide a comprehensibility and consistent terminology and help with Characterization of Energy
Efficiency related Information, assist in the development of the YANG data models at the different levels in the
IETF, bring clarity to the Energy efficiency related discussions between different groups within IETF or across
other across.

It will touch many aspects of energy efficiency and the vocabulary associated with those topics. It is not meant
to be a complete description of energy efficiency. The definitions in this document are not normative for IETF
standards; however, they are useful and standards may make informative reference to this document after it becomes
an RFC.  Some of the definitions in this document come from many earlier IETF documents. Some of other definitions
come from documents beyond the IETF.

# Terms and Definitions

The following terms are defined in this document:
Energy Efficiency
   The concept of energy efficiency refers to the ability to use available of energy to achieve a specific benefit
in a resource conserved manner and at low cost. The energy efficiency is ratio between the useful output and input
of an energy conversion process of network devices.

Energy Efficiency metrics
   A set of metrics that are used for evaluation of energy consumption and network performance characterize the
effectiveness of energy management strategy.

Energy Efficiency Ratio
The ratio of total throughput (system capacity) to the total power consumed (bits/Joule). It is the throughput forwarded
by 1 watt and it is introduced in [ETSI-ES-203-136].  A higher EER corresponds to a better the energy efficiency.

Power Usage Effectiveness
The metric used to measure data center energy efficiency. It is calculated by the ratio between the total energy
consumed by the data center and the energy needed for IT equipment.

Network level Energy Efficiency
Network level metrics are used to evaluate the energy efficiency of an entire network or part of it.

Device level Energy Efficiency
Equipment/system level metrics are mostly used to compare Network equipment of the same functionality and place in
a network. They evaluate the overall energy efficiency performance at the equipment/system level

Component Level Energy Efficiency
Component-level metrics can be used in the design, development and manufacture of energy efficient equipment. They
regard equipment as an "open box" and evaluate the energy efficiency performance of its individual components.
Measuring and understanding the energy efficiency or energy consumption of each component within the equipment
helps to identify the “hot spots” and key components in a system with regard to energy saving.

# Standards Bodies and Standards

This section describes some of the standards bodies and standards that appear in discussions of energy efficiency
in the IETF.  This is an incomplete and possibly over-full list; listing too few bodies or standards can be just
as politically dangerous as listing too many.  Note that there are many other bodies that deal with energy
efficiency; however, few if any of them appear commonly in IETF standards work.

## Standard bodies

ITU-T SG5

ITU-T Study Group 5 (SG5) has already worked on developing standards on energy efficiency before IETF is started.
ITU-T SG5 has many diverse standards in the environment efficiency field. These standards include L.1310, L.1315,
L.1316, L.1320 covering energy efficiency terminology, framework, metrics and measurement method.
In addition, ITU-T SG5 is also is responsible for other standards that might be of interest to protocol developers
and network operators. L.1331 specifies Assessment of mobile network energy efficiency.L.1333 specifies the
correlation between the carbon intensity indicator and energy efficiency metric. The carbon KPI defined in L.1333
refers to the energy efficiency metric defined in ITU-T L.1331. ITU-T L.1410 deals with the assessment of the
environmental impact of information and communication technology (ICT) goods, networks and services. It provides
specific guidance on energy and greenhouse gas (GHG) impacts.


ETSI TCEE
ETSI Technical Committee (TC) Environment Engineering (EE) is working together with ITU-T SG5 to develop technically
aligned standards on energy efficiency and environment aspect. These standards include energy efficiency, power
feeding solution, circular economy and network efficiency KPI and eco-design requirement for ICT, with the aim to
build an international eco-environmental standardization. ETSI ES 203 106 defines the energy consumption metrics and
measurement methods for router and Ethernet switch equipment. It specifies the methodology and the test conditions to
measure the power consumption of router and switch equipment and is also applicable to Core, edge and access routers.


3GPP SA5
3GPP SA5 has, in Release 17, extended its scope from RAN only to the whole 5G system and worked on Energy Efficiency
(EE) and Energy saving (ES) of mobile networks. EE Key Performance Indicators (KPI) have been defined for the 5G core
network and network slices.
As for RAN, their Energy Efficiency is defined by their performance divided by their Energy Consumption (EC), where
the definition of the performance depends on the type of network entity it applies to. From this, SA5 work aimed at
defining the best metrics for each of them, and their measurement method.
During Rel-18, WG SA5 works with ETSI NFV to explore more accurate virtual CPU usage measurements from ETSI NFV MANO,
Introduce additional metrics when estimating the Energy Consumption of Virtual Machines, e.g. their virtual disk or
link usage. In addition new use cases for Energy Saving, applied to NG-RAN, 5GC and network slicing, AI/ML assisted
energy saving scenarios are also investigated.

## Energy efficiency Metrics and Measurement Method

Metric for wireless access technologies
EERFU= Eoutput/ERPU
Where Eoutput is daily RF output energy consumption under different load
ERFU is daily RF units energy consumption under different load.

Metric for routers and Ethernet switches
 EER=Ti/Pw [Mbit/s/W]
Where Ti is NDR throughput, Pw is weighted power

Metric for small network devices
 EER=0.35Tidle+0.5Tlowpower+-.15TMaximum/
     0.35Pidle+0.5Plowpower_0.15Pmaximum
Where throughput is maximum non drop data rate beween wide area Network and
local area network kport in the ingress direction;
Line rate/speed is maximum possible number of transmitted/received bits.

Metric for power equipment
δ=Po/Pi
where Po is output power, Pi is input power. This energy efficiency value is
measured or calculated from the testing data over specified time period.

Metric for cooling equipment
η=Qt/Pi
whereηis the energy efficiency of the air conditioner
Pi is the input power,Qt is the sum of the sensible cooling capacity and the
latent cooling capacity.

# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.