---
title: "Optimization Techniques for Heterogenous Hadoop Distributed File Systems"
collection: publications
permalink: /publications/hdpopt
excerpt: 'This article discusses and shares results of optimization techniques centered around Hadoop File Systems having disks of varied generations'
date: 2019-10-21
paperurl: ''
---
## Abstract
The MapReduce framework has gained wide popularity as a scalable distributed system environment for efficient processing of large scale data of the order of Terabytes or more. Hadoop, open source implementation of MapReduce coupled with Hadoop Distributed File System, is widely applied to support cluster computing jobs requiring low response time. The current Hadoop implementation assumes that nodes in the cluster are homogenous in nature. Data locality and placement has not ben taken into account for launching speculative processing tasks. Furthermore, every node in the cluster is assumed to have same I/O speed despite some of the nodes being configured using vastly varying generation of storage hardware. Also, network delays being incurred due to data movement during run time have been ignored in the recent Hadoop implementations. Unfortunately,
both the homogeneity and data locality assumptions in Hadoop are optimistic at best and unachievable at worst, potentially introducing performance problems in data centers. This article explores the Hadoop data placement policy in detail and proposes a modified block placement policy that increases the efficiency
of the overall system. Also, the idea of placing data across the cluster in a way that a node possessing higher I/O capabilities is allocated more data is addressed, thereby reducing inter-node traffic and increasing overall performance.
