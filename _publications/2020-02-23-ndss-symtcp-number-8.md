---
title: "SymTCP: Eluding Stateful Deep Packet Inspection with Automated Discrepancy Discovery"
collection: publications
permalink: /publication/2020-02-23-ndss-symtcp
excerpt: ''
date: 2020-02-23
venue: 'Network & Distributed System Security Symposium (NDSS) 2020'
paperurl: ''
authors: 'Zhongjie Wang, Shitong Zhu, Yue Cao, Zhiyun Qian, Chengyu Song, Srikanth V. Krishnamurthy, Kevin S. Chan, and Tracy D. Braun'
citation: 'Zhongjie Wang, Shitong Zhu, Yue Cao, Zhiyun Qian, Chengyu Song, Srikanth V. Krishnamurthy, Kevin S. Chan, and Tracy D. Braun. 2020. SymTCP: Eluding Stateful Deep Packet Inspection with Automated Discrepancy Discovery. In Network and Distributed Systems Security (NDSS) Symposium 2020, 23-26 February 2020, San Diego, CA, USA. https://dx.doi.org/10.14722/ndss.2020.24083'
---
A key characteristic of commonly deployed deep packet inspection (DPI) systems is that they implement a simpli- fied state machine of the network stack that often differs from that of endhosts. The discrepancies between the two state machines have been exploited to bypass such DPI based middleboxes. However, most prior approaches to do so rely on manually crafted adversarial packets, which not only are labor-intensive but may not work well across a plurality of DPI-based middleboxes. Our goal in this work is to develop an automated way to craft candidate adversarial packets, targeting TCP implementations in particular. Our approach to achieving this goal hinges on the key insight that while the TCP state machines of DPI implementations are obscure, those of the endhosts are well established. Thus, in our system SYMTCP, using symbolic execution, we systematically explore the TCP implementation of an endhost, identifying candidate packets that can reach critical points in the code (e.g., which causes the packets to be accepted or dropped/ignored); such automatically identified packets are then fed through the DPI middlebox to determine if a discrepancy is induced and the middlebox can be eluded. We find that our approach is extremely effective. It can generate tens of thousands of candidate adversarial packets in less than an hour. When evaluating against multiple state-of-the-art DPI systems such as Zeek and Snort, as well as a state-level censorship system, viz. the Great Firewall of China, we identify not only previously known evasion strategies, but also novel ones that were never previously reported (e.g., involving the urgent pointer). The system can be extended easily towards other combinations of operating systems and DPI middleboxes, and serves as a valuable tool for testing future DPIs’ robustness against evasion attempts.

[Download paper here](https://zhongjie.me/files/ndss20_symtcp.pdf)

[Download slides here](https://zhongjie.me/files/ndss20_symtcp_slides.pdf)

[Source code](https://github.com/seclab-ucr/SymTCP)


