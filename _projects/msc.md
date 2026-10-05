---
layout: page
title: MSC
description: High-Throughput Parallel File Transfer for Linux
img: assets/img/projects/msc/mscReliability.png
importance: 0
category: "2026"
related_publications: false
---

MSC (Multi-Socket Copy) is a command-line tool, written in C, for moving large files and directory trees between Linux hosts as fast as the network allows. It launches its peer over SSH, then splits the transfer across many parallel flows carried over reliable UDP, with its own congestion control, pacing, path-MTU discovery, and checkpoint/resume so an interrupted transfer can pick up where it left off. A TCP data transport and optional Lustre support are also available.

I helped write MSC during my summer 2026 High Performance Computing internship at the National Security Agency, where it was built to replace the agency's incumbent file transfer utility and outperformed every alternative we benchmarked. Its default congestion controller keys on delivery rate and minimum round-trip time rather than packet loss, which avoids the throughput collapse that loss-based controllers suffer on high-bandwidth, high-latency paths. Loss-based Reno and CUBIC controllers are included for comparison, and the controller interface is pluggable, so new algorithms can be implemented and tested against real file transfers without a second host.

After agency review, MSC was released as open source under the MIT License, and I am now one of its maintainers. The source and documentation are on [GitHub](https://github.com/fcsi-msc/msc).
