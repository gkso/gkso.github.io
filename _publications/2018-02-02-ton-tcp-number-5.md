---
title: "Off-Path TCP Exploits of the Challenge ACK Global Rate Limit"
collection: publications
permalink: /publication/2018-02-02-ton-tcp-offpath
excerpt: ''
date: 2018-02-02
venue: 'IEEE/ACM Transactions on Networking'
paperurl: ''
authors: 'Yue Cao, Zhiyun Qian, Zhongjie Wang, Tuan Dao, Srikanth V. Krishnamurthy, and Lisa M. Marvel'
citation: 'Y. Cao, Z. Qian, Z. Wang, T. Dao, S. V. Krishnamurthy and L. M. Marvel, "Off-Path TCP Exploits of the Challenge ACK Global Rate Limit," in IEEE/ACM Transactions on Networking, vol. 26, no. 2, pp. 765-778, April 2018. doi: 10.1109/TNET.2018.2797081'
---
In this paper, we report a subtle yet serious side channel vulnerability (CVE-2016-5696) introduced in a recent transmission control protocol (TCP) specification. The specification is faithfully implemented in Linux kernel version 3.6 (from 2012) and beyond, and affects a wide range of devices and hosts. In a nutshell, the vulnerability allows a blind off-path attacker to infer if any two arbitrary hosts on the Internet are communicating using a TCP connection. Further, if the connection is present, such an off-path attacker can also infer the TCP sequence numbers in use, from both sides of the connection; this in turn allows the attacker to cause connection termination and perform data injection attacks. We illustrate how the attack can be leveraged to disrupt or degrade the privacy guarantees of an anonymity network such as Tor, and perform web connection hijacking. Through extensive experiments, we show that the attack is fast and reliable. On average, it takes about 40 to 60 s to finish and the success rate is 88% to 97%. Finally, we propose changes to both the TCP specification and implementation to eliminate the root cause of the problem.

[Download paper here](https://zhongjie.me/files/ton18_tcp_offpath.pdf)

