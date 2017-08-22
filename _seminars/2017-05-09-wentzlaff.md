---
layout: post
title: Processors for the Data Center and Cloud of the Future
subtitle:
memento: http://memento.epfl.ch/event/processors-for-the-data-center-and-cloud-of-the-fu/
speaker: David Wentzlaff
speaker-web: https://www.princeton.edu/~wentzlaf/
image: wentzlaff.jpg
---
Current-day data centers and IaaS clouds (e.g. Amazon EC2, MS Azure, Google GCE) use microprocessors that are very similar to or the same as those used in small servers and desktops.  This work rethinks the design of microprocessors specifically for data center use along with how microprocessors are affected by the novel economic models that have been popularized by IaaS clouds.  This talk will describe several architectural changes including how a processor can be decomposed into sub-components (e.g. ALU, Cache, Fetch Unit) that can be individually rented in IaaS clouds, how running similar programs can be taken advantage of in the data center, how architectural features such as the flavor of memory bandwidth (bursty vs. bulk) can be provisioned and sold in the data center, and novel memory architectures that enable the creation of sub-coherence domains of cache coherence across the data center.  This work has not only been simulated, but many of the discussed ideas have been implemented in one of the largest academic processors ever built, the Princeton Piton Processor.  Piton is a 25-core manycore built in IBM's 32nm process technology containing over 460 Million transistors and runs full stack Debian Linux with networking.   This talk will discuss Piton along with what it takes to tape-out a complex microprocessor in an academic setting.  Last, Piton has been recently open sourced as the OpenPiton (http://www.openpiton.org) project which is a expandable manycore platform which includes RTL, thousands of tests, and implementation scripts.  The talk will conclude by discussing how OpenPiton is able to contribute to the burgeoning field of open source hardware.
