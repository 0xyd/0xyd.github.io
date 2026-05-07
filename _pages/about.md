---
permalink: /
title: "About Yu De"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a PhD student at [CISPA Helmholtz Center for Information Security](https://cispa.de), Germany, and a group member of [SCy-Phy](https://scy-phy.net/), led by [Dr. Nils Ole Tippenhauer](https://tippenhauer.de/). In 2022, I received my M.Sc. in Computer Science from [Saarland University](https://www.uni-saarland.de). Before moving to Germany, I studied Mechanical Engineering at [Chang Gung University](https://www.cgu.edu.tw), Taiwan.

My main research topics are system security, specifically physical-layer side-channel analysis, Edge AI, and fuzz testing. I am also interested in machine learning, especially its applications in the security domain. In my free time, I like to go bouldering and do some weight training. Recently, I started my journey with the electric guitar!

Research Work
===

### Theft in the Frequency Domain: Stealing Embedded DNN Architecture via a Single Power Side-Channel Trace

**Authors:** Yu-De Lin, Yi Han, Dymytriy Zyunkin, Saman Aliari Zonouz, Nils Ole Tippenhauer
**Venue:** ESORICS 2026 (Under Review)

<!-- Recent advancements have enabled the deployment of highly optimized deep neural networks (DNNs) on embedded systems, where MCU-based models are especially valuable because their design and training require extensive data and computational resources. However, these models are vulnerable to physical side-channel model-stealing attacks, in which attackers record power traces while querying victim devices to extract deployed models. Existing CPA-like methods require millions of queries, while DNN-based architecture-extraction approaches need fewer queries but rely on restrictive assumptions about architectural parameters; overall, even minor architectural differences can significantly degrade the stolen model’s performance. To address both strong architectural assumptions and high query requirements while maintaining high extraction precision, we propose Flow Tracing Attack, which extracts the full architecture of an embedded DNN from as few traces as possible without requiring any prior assumptions about the architecture parameters. By applying wavelet-based time-frequency analysis to Flows of Interest, signal sequences characteristic of specific neural network operations, Flow Tracing Attack identifies different neural network layers and reconstructs the model architecture. On average, surrogate models reconstructed by Flow Tracing Attack recover 97.25% of the victims' accuracy. -->

### Execution Divergence Graphs: Effective Discovery of Control-Flows from Execution Traces as Fuzzing Feedback

**Authors:** Yu-De Lin, Nils Ole Tippenhauer
**Venue:** RAID 2026 (Under Review)
<!-- 
Fuzz testing is widely used for security testing of proprietary software, with efficient strategies typically relying on execution feedback to guide input generation when basic blocks can be directly observed and instrumented. However, such feedback is unavailable in scenarios such as in-situ fuzzing of black-box devices or fuzzing obfuscated compiled binaries. In this work, we explore approaches for guiding fuzzers using feedback derived from a control-flow-graph-like (CFG-like) structure constructed from runtime execution. We first outline a simple divergence-detection method for identifying unique execution traces, then present an improved approach based on an Execution Divergence Graph (EDG). We implement both methods and show that they outperform a baseline blind fuzzer, while also addressing challenges such as repeated code execution in loops, which the EDG-based approach handles effectively. Finally, we demonstrate effective fuzzing of several obfuscated targets, compare performance in settings where static instrumentation is impossible, and note that although our focus is on scenarios where full instruction traces are directly observable, the scheme can also be applied with other feedback channels, such as power consumption. -->

