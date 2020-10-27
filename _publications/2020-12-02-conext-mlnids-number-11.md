---
title: "You Do (Not) Belong Here: Detecting DPI Evasion Attacks with Context Learning"
collection: publications
permalink: /publication/2020-12-02-conext-ml-nids
excerpt: ''
date: 2020-12-02
venue: 'ACM CoNEXT 2020'
paperurl: ''
authors: 'Shitong Zhu, Shasha Li, Zhongjie Wang, Xun Chen, Zhiyun Qian, Srikanth V. Krishnamurthy, Kevin S. Chan, Ananthram Swami'
citation: ''
---
As Deep Packet Inspection (DPI) middleboxes become increasingly popular, a spectrum of adversarial attacks have emerged with the goal of evading such middleboxes. Many of these attacks exploit discrepancies between the middlebox network protocol implementations, and the more rigorous/complete versions implemented at end hosts. These evasion attacks largely involve subtle manipulations of packets to cause different behaviours at DPI and end hosts, to cloak malicious network traffic that is otherwise detectable. With recent automated discovery, it has become prohibitively challenging to manually curate rules for detecting these manipulations. In this work, we propose CLAP, the first fully-automated, unsupervised ML solution to accurately detect and localize DPI evasion attacks. By learning what we call the packet context, which essentially captures inter-relationships across both (1) different packets in a connection; and (2) different header fields within each packet, from benign traffic traces only, CLAP can detect and pinpoint packets that violate the benign packet contexts (which are the ones that are specially crafted for evasion purposes). Our evaluations with 73 state-of-the-art DPI evasion attacks show that CLAP achieves an Area Under the Receiver Operating Characteristic Curve (AUC-ROC) of 0.963, an Equal Error Rate (EER) of only 0.061 in detection, and an accuracy of 94.6% in localization. These results suggest that CLAP can be a promising tool for thwarting DPI evasion attacks.

[Download paper here](https://zhongjie.me/files/conext20_ml_nids.pdf)

