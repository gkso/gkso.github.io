---
title: "Eluding ML-based Adblockers With Actionable Adversarial Examples"
collection: publications
permalink: /publication/2021-12-06-acsac-a4
excerpt: ''
date: 2021-12-06
venue: '37th Annual Computer Security Applications Conference (ACSAC)'
paperurl: ''
authors: 'Shitong Zhu, Zhongjie Wang, Xun Chen, Shasha Li, Keyu Man, Umar Iqbal, Zhiyun Qian, Kevin Chan, Srikanth V. Krishnamurthy, Zubair Shafiq, Yu Hao, Guoren Li, Zheng Zhang, Xiaochen Zou'
---
Online advertisers have been quite successful in circumventing traditional adblockers that rely on manually curated rules to detect ads. As a result, adblockers have started to use machine learning (ML)classifiers for more robust detection and blocking of ads. Among these, AdGraph which leverages rich contextual information to classify ads, is arguably, the state of the art ML-based adblocker. In this paper, we present A4, a tool that intelligently crafts adversarial ads to evade AdGraph. Unlike traditional adversarial examples in the computer vision domain that can perturb any pixels (i.e.,unconstrained), adversarial ads generated by A4 are actionable in the sense that they preserve the application semantics of the webpage. Through a series of experiments we show that A4 can bypass AdGraph about 81% of the time, which surpasses the state-of-the-art attack by a significant margin of 145.5%, with an overhead of <20% and perturbations that are visually imperceptible in the rendered webpage. We envision that A4’s framework can be used to potentially launch adversarial attacks against other ML-based web applications.

