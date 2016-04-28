---
layout: page
title: Portfolio
permalink: /portfolio/
---


### **IPv4 & IPv6 Duality and Anomaly Detection**


 The duality project was completed for the Computer & Network Security
 course at the University of Oregon, inspired by a PHD student's 
 proposal. The purpose of this project is to compare and contrast 
 networking information for both IPv4 and IPv6, in an attempt to learn
 more about network topologies and how they affect routing security. 
 Our topological understanding is based on routing paths as well as 
 autonomous system (AS) paths. The project has two major components for
 gathering path data. Routing paths are gathered using traceroutes through
 both IPv4 and IPv6, whereas AS paths are parsed out of routing tables 
 specific to each protocol. Each component is explained in more detail
 below. The intended use of this suite is to further our understanding of
 anamalous border gateway prtocol (BGP) outages and their detectability. 
 Note, this project is an analytic tool for conducting future BGP research
 and does not provide a direct means of anomaly detection.

![Poster screenshot]({{ site.baseurl }}/assets/duality_project_poster.jpg)

**Traceroute Comparison**

 The first portion of the project involves the comparison of IPv4 and IPv6
 traceroute results for each of Alexa's top 500 websites that currently 
 support both protocols. Our goal was to compare daily traceroute results 
 for each protocol based on hop count and variability, in an attempt 
 explore routing paths for several autonomous systems. This functionality 
 is provided by a Python program that runs IPv4 and IPv6 traceroutes on 
 given domains, storing results in newly created files. An auxiliary 
 program then processes the files and generates diagnostic information 
 about which IP addresses were seen and how often. A batch script drives 
 the traceroute routine through the list of top websites and optionally 
 updates diagnostic files.


**IPv4 & IPv6 Makes BGP Anomaly Detection Difficult**

 Routing information base (RIB) tables store topological information about
 a router's "neighbors." Our approach to studying BGP behavior is to 
 understand how this topology has changed over time, especially during known
 outages. Several terabytes worth of RIB tables are currently being collected
 and stored by the University of Oregon Route Views Archive Project designed 
 by David Meyer. Using these RIB tables, we are able to compare AS paths for
 both IPv4 and IPv6 by searching for all paths that share source and 
 destination adresses. Systems governed by BGP are still susceptible to 
 routing attacks such as blackholes, BGP rerouting, and BGP spoofing. Moving
 forward, we plan to analyze BGP behavior during past events where routing
 attacks were believed to be the cause of specific outages. 





