---
title: "Principled Unearthing of TCP Side Channel Vulnerabilities"
collection: publications
permalink: /publication/2019-11-11-ccs-tcp-model-checking
excerpt: ''
date: 2019-11-11
venue: '26th ACM Conference on Computer and Communications Security (CCS)'
paperurl: ''
authors: 'Yue Cao, Zhongjie Wang, Zhiyun Qian, Chengyu Song, Srikanth V. Krishnamurthy, and Paul Yu'
citation: 'Yue Cao, Zhongjie Wang, Zhiyun Qian, Chengyu Song, Srikanth V. Krishnamurthy, and Paul Yu. 2019. Principled Unearthing of TCP Side Channel Vulnerabilities. In Proceedings of the 2019 ACM SIGSAC Conference on Computer and Communications Security (CCS ’19). Association for Computing Machinery, New York, NY, USA, 211–224. DOI:https://doi.org/10.1145/3319535.3354250'
---
Recent work has showcased the presence of subtle TCP side channels in modern operating systems, that can be exploited by off-path adversaries to launch pernicious attacks such as hijacking a connection. Unfortunately, most work to date is on the manual discovery of such side-channels, and patching them subsequently. In this work we ask "Can we develop a principled approach that can lead to the automated discovery of such hard-to-find TCP side-channels?" We identify that the crux of why such side-channels exist is the violation of the non-interference property between simultaneous TCP connections i.e., there exist cases wherein a change in state of one connection implicitly leaks some information to a different connection (controlled possibly by an attacker). To find such non-interference property violations, we argue that model-checking is a natural fit. However, because of limitations with regards to its scalability, there exist many challenges in using model checking. Specifically, these challenges relate to (a) making the TCP code base self-contained and amenable to model checking and (b) limiting the search space of model checking and yet achieving reasonable levels of code coverage. We develop a tool that we call SCENT (for Side Channel Excavation Tool) that addresses these challenges in a mostly automated way. At the heart of SCENT is an automated downscaling component that transforms the TCP code base in a consistent way to achieve both a reduction in the state space complexity encountered by the model checker and the number and types of inputs needed for verification. Our extensive evaluations show that SCENT leads to the discovery of 12 new side channel vulnerabilities in the Linux and FreeBSD kernels. In particular, a real world validation with one class of vulnerabilities shows that an off-path attacker is able to infer whether two arbitrary hosts are communicating with each other, within slightly more than 1 minute, on average.

[Download paper here](https://zhongjie.me/files/ccs19_tcp_model_checking.pdf)

