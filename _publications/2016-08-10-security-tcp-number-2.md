---
title: "Off-Path TCP Exploits: Global Rate Limit Considered Dangerous"
collection: publications
permalink: /publication/2016-08-10-security-tcp
excerpt: ''
date: 2016-08-10
venue: '25th USENIX Security Symposium'
paperurl: ''
authors: 'Yue Cao, Zhiyun Qian, Zhongjie Wang, Tuan Dao, Srikanth V. Krishnamurthy, and Lisa M. Marvel'
citation: 'Yue Cao, Zhiyun Qian, Zhongjie Wang, Tuan Dao, Srikanth V. Krishnamurthy, and Lisa M. Marvel. 2016. Off-path TCP exploits: global rate limit considered dangerous. In Proceedings of the 25th USENIX Conference on Security Symposium (SEC’16). USENIX Association, USA, 209–225.'
---
In this paper, we report a subtle yet serious side channel vulnerability (CVE-2016-5696) introduced in a recent TCP specification. The specification is faithfully implemented in Linux kernel version 3.6 (from 2012) and beyond, and affects a wide range of devices and hosts. In a nutshell, the vulnerability allows a blind off-path attacker to infer if any two arbitrary hosts on the Internet are communicating using a TCP connection. Further, if the connection is present, such an off-path attacker can also infer the TCP sequence numbers in use, from both sides of the connection; this in turn allows the attacker to cause connection termination and perform data injection attacks. We illustrate how the attack can be leveraged to disrupt or degrade the privacy guarantees of an anonymity network such as Tor, and perform web connection hijacking. Through extensive experiments, we show that the attack is fast and reliable. On average, it takes about 40 to 60 seconds to finish and the success rate is 88% to 97%. Finally, we propose changes to both the TCP specification and implementation to eliminate the root cause of the problem.

[Download paper here](https://zhongjie.me/files/sec16_tcp_offpath.pdf)

