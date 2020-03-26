---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* B.Eng. in Information Security, Beijing University of Posts and Telecommunications, 2009
* M.Sc. in Computer Architecture, Peking University, 2012
* Ph.D. in Computer Science, University of California, Riverside, 2020 (expected)

Work experience
======
* Summer 2019: Research Intern, Samsung Research America
  * Exploring statefulness of mobile Trusted Applications and their control flow dependance using Symbolic Execution technique. Automated bug finding.

* Summer 2018: Research Intern, International Computer Science Institute (ICSI) at Berkeley
  * Offloading network protocol identification from Bro to programmable NIC. Prototype implemented in Zeek (formerly known as Bro).

* March 2015 - June 2015: Data Analyst, Maxent, Inc.
  * Analyzing tera-scale user data of mobile customers
  * Building and maintaining data warehouse on HDFS+Hive+Spark

* July 2012 - May 2014: Advanced Software Development Engineer in Test, NetEase, Inc.
  * Developed automatic source code analysis platform, which performs static code analysis on multiple projects concurrently and automatically
  * Developed real-time code coverage testing tool, which traces the code execution of both server-side and client-side, then presents the executions of code lines in real time
  * Designed and conducted automatic tests and stress tests for MMORPG (Massively Multiplayer Online Role Playing Game) with 10000+ concurrent players

* Summer 2011: Technology & Data Intern, Morgan Stanley
  * Developed a backend module for equity trading system, which executes post-trade position verification using finite state machines

* November 2008 – May 2009: Research Intern, Microsoft Research Asia
  * Devised a distributed key-value retrieval algorithm using MapReduce and B+ Tree
  * Designed and implemented a ranking algorithm based on distributed random walk using MapReduce on a cluster of hundreds of machines
  * Devised algorithms to measure similarity between search queries
  
Skills
======
* Symbolic Execution (S2E, angr)
* Static Program Analysis (LLVM)
* Reverse Engineering (IDA Pro, Ghidra)
* Network Protocol Analysis
* Programming
  * Python
  * C/C++

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>


For a PDF version, click [here](https://zhongjie.me/files/CV_ZhongjieWang_2020.pdf).

