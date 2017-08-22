---
layout: project
title: soNUMA
subtitle: Scale-Out NUMA
website: http://parsa.epfl.ch/sonuma.html
---

Emerging datacenter applications operate on vast datasets that are kept in DRAM to minimize latency. The large number of servers needed to accommodate this massive mem- ory footprint requires frequent server-to-server communication in applications such as key-value stores and graph-based applications that rely on large irregular data structures. The fine-grained nature of the accesses is a poor match to commodity networking technologies, including RDMA, which incur delays of 10-1000x over local DRAM operations. Scale-Out NUMA is an architecture, programming model, and communication protocol for low-latency, distributed in-memory processing, designed to bridge the latency gap between local and remote memory access.