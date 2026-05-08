---
permalink: /
title: "About Yu De"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a PhD student at [CISPA Helmholtz Center for Information Security](https://cispa.de), Germany, and a group member of [SCy-Phy](https://scy-phy.net/), led by [Dr. Nils Ole Tippenhauer](https://tippenhauer.de/). In 2022, I received my M.Sc. in Computer Science from [Saarland University](https://www.uni-saarland.de). Before moving to Germany, I was working in [CyberSecurity Technology Institute](https://www.iii.org.tw/about/organization/departments/ae427346-e401-4f57-8b90-6df47504c361), Taiwan, as a junior engineer. I acquired my Bachelor degree of Mechanical Engineering at [Chang Gung University](https://www.cgu.edu.tw)


My research focuses on how physical-layer side channels can infringe the security of a system. We investigate how such side channels can be leveraged to compromise system security, for example, by stealing DNNs deployed on edge devices. We are also working on using physical-layer side-channel feedback to guide fuzzers for effectively testing hardware devices. Besides physical-layer side channels, I am also interested in machine learning, especially its applications in the security domain.

When I was in Taiwan, I liked to participate in open-source communities such as g0v and work on civic tech projects. I also helped organizing PyCon TW 2015 and 2016 as a program officer. Now in Germany, I have acquired several new habits, such as bouldering, weight training, and playing electric guitar.


Research Work
===

### Theft in the Frequency Domain: Stealing Embedded DNN Architecture via a Single Power Side-Channel Trace

**Authors:** Yu-De Lin, Yi Han, Dymytriy Zyunkin, Saman Aliari Zonouz, Nils Ole Tippenhauer
**Venue:** ESORICS 2026 (Under Review)

Recent advancements have enabled the deployment of highly optimized deep neural networks (DNNs) on embedded systems, where MCU-based models are especially valuable due to the extensive data and computational resources required for their design and training. However, these models are vulnerable to physical side-channel model-stealing attacks, where attackers record power traces while querying victim devices to extract deployed models. Existing CPA-like methods require millions of queries, while DNN-based architecture-extraction methods require fewer queries but rely on restrictive assumptions about architectural parameters. To address these limitations, we propose Flow Tracing Attack, which extracts the full architecture of an embedded DNN from as few traces as possible without requiring prior assumptions about the architecture parameters. 

### Execution Divergence Graphs: Effective Discovery of Control-Flows from Execution Traces as Fuzzing Feedback

**Authors:** Yu-De Lin, Nils Ole Tippenhauer
**Venue:** RAID 2026 (Under Review)

Fuzz testing is widely used for security testing of proprietary software, but effective feedback-driven strategies are difficult to apply when basic blocks cannot be directly observed or instrumented, such as in in-situ fuzzing of black-box devices or fuzzing obfuscated binaries. In this work, we explore ways to guide fuzzers using feedback from a control-flow-graph-like structure constructed from runtime execution, starting with a simple divergence-detection method and then introducing an improved Execution Divergence Graph (EDG)-based approach. We implement both methods and show that they outperform a baseline blind fuzzer, handle challenges such as repeated code execution in loops, and enable effective fuzzing of obfuscated targets, with the potential to support other feedback channels such as power consumption.

### Powerfuzz: Efficient Power Side-Channel Guided Fuzzing of Proprietary Embedded Systems with Execution Divergence Graphs

**Authors:** Yu-De Lin, Till Schlüter, Pouya Narimani, Ali Abbasi, Nils Ole Tippenhauer

State-of-the-art fuzzers use real-time control-flow feedback to maximize code coverage, but this feedback is unavailable for proprietary embedded firmware that cannot be instrumented on-device or re-hosted in emulation because neither the source code nor the binary is accessible. In this work, we replace instrumentation feedback with a power-based side channel for in-situ fuzzing, using the core insight that novel sections in power traces can indicate novel code execution without requiring prior knowledge of the code or detection of individual instructions.

Master Thesis
===

### Extracting DNN Models from Embedded Devices via Power and Timing Side-channels

**Advisors:** Dr. Nils Ole Tippenhauer, Prof. Dr. Jan Reineke.

As hardware becomes increasingly powerful, running DNNs on embedded devices has become common in the era of edge computing, but the limited security protection on such devices puts the intellectual property of deployed AI models at high risk of being stolen through model extraction attacks. Prior work has shown that attackers can steal model functionality without prior knowledge, use data from different distributions through strategies such as Knockoff Nets, and exploit physical-layer side channels such as power. This thesis focuses on power and timing side channels, first demonstrating information leakage through simple power analysis and then proposing a Monte Carlo-based NAS attack that combines Knockoff Nets with timing side-channel analysis to recover models with performance and execution time close to the victim model.


Projects and Tools
===

### Hiwi: Embedding Leakage
**Year**: 2019

A research project that investigates whether word embeddings can leak sensitive information.

### Hiwi: Extraction Attack on LMs
**Year**: 2019

Implemented an extraction attack on Language Models (LMs).

### Sneak
**Year**: 2018 [**GitHub**](https://github.com/0xyd/Sneak)

Sneak is a URL transfer tool based on Tor technology.

### Visualized Judicial Data
**Year**: 2015 [**GitHub**](https://github.com/0xyd/VisualJusticeTW) 

Visualizes statistical data provided by judicial institutions in Taiwan.

### Social Authentication in Django
**Year**: 2014 [**GitHub**](https://github.com/0xyd/SocialAuthDjangoTutorial)

A beginner tutorial for social authentication in the Django framework.