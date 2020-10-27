---
title: "Your State is Not Mine: A Closer Look at Evading Stateful Internet Censorship"
collection: publications
permalink: /publication/2017-11-01-imc-censorship
excerpt: ''
date: 2017-11-01
venue: 'ACM Internet Measurement Conference (IMC) 2017'
paperurl: ''
authors: 'Zhongjie Wang, Yue Cao, Zhiyun Qian, Chengyu Song, and Srikanth V. Krishnamurthy'
citation: 'Zhongjie Wang, Yue Cao, Zhiyun Qian, Chengyu Song, and Srikanth V. Krishnamurthy. 2017. Your state is not mine: a closer look at evading stateful internet censorship. In Proceedings of the 2017 Internet Measurement Conference (IMC ’17). Association for Computing Machinery, New York, NY, USA, 114–127. DOI:https://doi.org/10.1145/3131365.3131374'
---
Understanding the behaviors of, and evading state-level Internet-scale censorship systems such as the Great Firewall (GFW) of China, has emerged as a research problem of great interest. One line of evasion is the development of techniques that leverage the possibility that the TCP state maintained on the GFW may not represent the state at end-hosts. In this paper we undertake, arguably, the most extensive measurement study on TCP-level GFW evasion techniques, with several vantage points within and outside China, and with clients subscribed to multiple ISPs. We find that the state-of-the art evasion techniques are no longer very effective on the GFW. Our study further reveals that the primary reason that causes these failures is the evolution of GFW over time. In addition, other factors such as the presence of middleboxes on the route from the client to the server also contribute to previously unexpected behaviors.

Our measurement study leads us to new understandings of the GFW and new evasion techniques. Evaluations of our new evasion strategies show that our new techniques provide much higher success rates of (compared to prior schemes) ≈ 90% or higher. Our results further validate our new understandings of the GFW's evolved behaviors. We also develop a measurement-driven tool INTANG, that systematically looks for and finds the best strategy that works with a server and network path. Our measurements show that INTANG can yield near perfect evasion rates and is extremely effective in aiding various protocols such as HTTP, DNS over TCP, and Tor in evading the GFW.

[Download paper here](https://zhongjie.me/files/imc17_censorship.pdf)

