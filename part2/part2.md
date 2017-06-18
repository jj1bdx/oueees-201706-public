autoscale: true
footer: Kenji Rikitake / oueees 201706 part 2 20-JUN-2017
slidenumbers: true

![](nasa-43569-slide.jpg)

# oueees-201706 Part 2: Distributed system fiasco

<!-- Use Deckset 1.8,1, Next theme, 4:3 aspect ratio -->

---

# Kenji Rikitake

20-JUN-2017
School of Engineering Science
Osaka University
Toyonaka, Osaka, Japan
@jj1bdx

Copyright ©2017 Kenji Rikitake.
This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

---

# Lecture notes on GitHub

* [https://github.com/jj1bdx/oueees-201706-public/](https://github.com/jj1bdx/oueees-201706-public/)
* Don't forget to *check out the issues*!

---

![original](rayi-christian-wicaksono-366-slide.jpg)

# [fit] Modern computing
## is
# [fit]cloud computing

---

![original fit](Cloud_applications_SVG.jpg)

---

![fit](Cloud_applications_SVG.jpg)

# Is cloud really a uniform and single entity?

---

![right fit](kyoto-u-hpc-20170425.jpg)

# Web services are clusters of computers and networks

**Thousands or millions of servers connected together**

**A physical server is separated into multiple virtual machines**

---

![original](irina-blok-15361-slide.jpg)

# [fit] Networks

---

![right fit](network-nodes.png)

# Example of networks connecting multiple nodes

Reference: Baran, Paul. On Distributed Communications: I. Introduction to Distributed Communications Networks. Santa Monica, CA: RAND Corporation, 1964. <https://www.rand.org/pubs/research_memoranda/RM3420.html>. Figure 1 in Chapter 1.

All figures drawn by Kenji Rikitake

---

![right fit](network-centralized.png)

# Centralized network

All nodes are connected to the single core

One hop to the core

Two hops between non-core nodes

No communication path between the nodes if the core fails

---

![right fit](network-decentralized.png)

# Decentralized network

A few nodes are connected to the core

Some nodes are connected to local concentrated nodes

Hierarchical structure

---

![right fit](network-distributed.png)

# Distributed network

No core exists anymore

No hierarchical structure

Multiple redundant paths are available between two nodes

---

![original fit](netsplit.jpg)

---
[.autoscale: true]

Photo credits:

* All photos are modified and edited by Kenji Rikitake
* Photos are from Unsplash.com unless otherwise noted

* Title: NASA
* Modern Computing is Cloud Computing: Rayi Christian Wicaksono
* Cloud Computing: <https://commons.wikimedia.org/wiki/File:Cloud_applications_SVG.svg>, licensed under [Creative Commons CC0 1.0 Universal Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/deed.en)
* Web services are clusters of computers: Kenji Rikitake, at Kyoto University ACCMS, April 2017
* Networks: Irina Blok
* Netsplit: <https://commons.wikimedia.org/wiki/File:Netsplit_split.svg>, in public domain

<!-- coding: utf-8 -->
<!-- End: -->
