---
title: "Themis: Ambiguity-Aware Network Intrusion Detection based on Symbolic Model Comparison"
collection: publications
permalink: /publication/2021-11-15-ccs-themis
excerpt: ''
date: 2021-11-15
venue: '28th ACM Conference on Computer and Communications Security (CCS)'
paperurl: ''
authors: 'Zhongjie Wang, Shitong Zhu, Keyu Man, Pengxiong Zhu, Yu Hao, Zhiyun Qian, Srikanth V. Krishnamurthy, Tom La Porta, Michael J. De Lucia'
citation: 'Zhongjie Wang, Shitong Zhu, Keyu Man, Pengxiong Zhu, Yu Hao, Zhiyun Qian, Srikanth V. Krishnamurthy, Tom La Porta, Michael J. De Lucia. Themis: Ambiguity-Aware Network Intrusion Detection based on Symbolic Model Comparison. In Proceedings of the 2021 ACM SIGSAC Conference on Computer and Communications Security (CCS ’21). Association for Computing Machinery, Virtual Event, Republic of Korea. DOI:https://doi.org/10.1145/3460120.3484762'
---
Network intrusion detection systems (NIDS) can be evaded by carefully crafted packets that exploit implementation-level discrepancies between how they are processed on the NIDS and at the endhosts. These discrepancies arise due to the plethora of endhost implementations and evolutions thereof. It is prohibitive to proactively employ a large set of implementations at the NIDS and check incoming packets against all of those. Hence, NIDS typically choose simplified implementations that attempt to approximate and generalize across the different endhost implementations. Unfortunately, this solution is fundamentally flawed since such approximations are bound to have discrepancies with some endhost implementations. In this paper, we develop a lightweight system Themis, which empowers the NIDS in identifying these discrepancies and reactively forking its connection states when any packets with “ambiguities” are encountered. Specifically, Themis incorporates an offline phase in which it extracts models from various popular implementations using symbolic execution. During runtime, it maintains a nondeterministic finite automaton to keep track of the states for each possible implementation. Our extensive evaluations show that Themis is extremely effective and can detect all evasion attacks known to date, while consuming extremely low overhead. En route, we also discovered multiple previously unknown discrepancies that can be exploited to bypass current NIDS.

[Download paper here](https://zhongjie.me/files/ccs21_themis.pdf)

