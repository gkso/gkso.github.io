---
title: "Investigation of a Recent Linux TCP Stack Vulnerability at Scale"
collection: publications
permalink: /publication/2017-06-05-sigmetrics-cack
excerpt: ''
date: 2017-06-05
venue: 'ACM SIGMETRICS'
paperurl: ''
authors: 'Alan Quach*, Zhongjie Wang*, and Zhiyun Qian (*co-first author)'
citation: 'Alan Quach, Zhongjie Wang, and Zhiyun Qian. 2017. Investigation of the 2016 Linux TCP Stack Vulnerability at Scale. Proc. ACM Meas. Anal. Comput. Syst. 1, 1, Article 4 (June 2017), 19 pages. DOI:https://doi.org/10.1145/3084441'
---
To combat blind in-window attacks against TCP, changes proposed in RFC 5961 have been implemented by Linux since late 2012. While successfully eliminating the old vulnerabilities, the new TCP implementation was reported in August 2016 to have introduced a subtle yet serious security flaw. Assigned CVE-2016-5696, the flaw exploits the challenge ACK rate limiting feature that could allow an off-path attacker to infer the presence/absence of a TCP connection between two arbitrary hosts, terminate such a connection, and even inject payload into an unsecured TCP connection.

In this work, we perform a comprehensive measurement of the impact of the new vulnerability. This includes (1) tracking the vulnerable Internet servers, (2) monitoring the patch behavior over time, (3) picturing the overall security status of TCP stacks at scale. Towards this goal, we design a scalable measurement methodology to scan the Alexa top 1 million websites for almost 6 months. We also present how notifications impact the patching behavior, and compare the result with the Heartbleed and the Debian PRNG vulnerability. The measurement represents a valuable data point in understanding how Internet servers react to serious security flaws in the operating system kernel.

[Download paper here](https://zhongjie.me/files/sigmetrics17_cack_measurement.pdf)

