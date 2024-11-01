---
title: "DNS Cache Poisoning Attack Reloaded: Revolutions with Side Channels"
collection: publications
permalink: /publication/2020-11-11-ccs-dns-poisoning
excerpt: ''
date: 2020-11-11
venue: 'ACM CCS 2020'
paperurl: ''
authors: 'Keyu Man, Zhiyun Qian, Zhongjie Wang, Xiaofeng Zheng, Youjun Huang, Haixin Duan'
citation: 'Keyu Man, Zhiyun Qian, Zhongjie Wang, Xiaofeng Zheng, Youjun Huang, and Haixin Duan. 2020. DNS Cache Poisoning Attack Reloaded: Revolutions with Side Channels. In Proceedings of the 2020 ACM SIGSAC Conference on Computer and Communications Security (CCS ’20). Association for Computing Machinery, New York, NY, USA, 1337–1350. DOI:https://doi.org/10.1145/3372297.3417280'
---
In this paper, we report a series of flaws in the software stack that leads to a strong revival of DNS cache poisoning — a classic attack which is mitigated in practice with simple and effective randomization-based defenses such as randomized source port. To successfully poison a DNS cache on a typical server, an off-path adversary would need to send an impractical number of 2^32 spoofed responses simultaneously guessing the correct source port (16-bit) and transaction ID (16-bit). Surprisingly, we discover weaknesses that allow an adversary to "divide and conquer" the space by guessing the source port first and then the transaction ID (leading to only 2^16 + 2^16 spoofed responses). Even worse, we demonstrate a number of ways an adversary can extend the attack window which drastically improves the odds of success. The attack affects all layers of caches in the DNS infrastructure, such as DNS forwarder and resolver caches, and a wide range of DNS software stacks, including the most popular BIND, Unbound, and dnsmasq, running on top of Linux and potentially other operating systems. The major condition for a victim being vulnerable is that an OS and its network is configured to allow ICMP error replies. From our measurement, we find over 34% of the open resolver population on the Internet are vulnerable (and in particular 85% of the popular DNS services including Google's 8.8.8.8). Furthermore, we comprehensively validate the proposed attack with positive results against a variety of server configurations and network conditions that can affect the success of the attack, in both controlled experiments and a production DNS resolver (with authorization).

[Download paper here](https://zhongjie.me/files/ccs20_dns_poisoning.pdf)

