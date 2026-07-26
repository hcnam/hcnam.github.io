---
paper_key: nam_ndss26
title: "On the Security Risks of Memory Adaptation and Augmentation in Data-plane DoS Mitigation"
collection: publications
category: conferences
permalink: /publication/nam-ndss26/
excerpt: "We introduce 'Heracles attack' that uncover security risks in adaptive data-plane DoS defenses in programmable switches, and propose a new sketch mechnaism 'Shield' to mitigate Heracles attack."
date: 2026-02-24
venue: "Network and Distributed System Security Symposium (NDSS)"
location: "San Diego, CA, USA"
abbr: "NDSS"
tier: "Tier-1"
detail_page: true
authors: "**Hocheol Nam**, Daehyun Lim, Huancheng Zhou, Guofei Gu, and Min Suk Kang"
paperurl: "/files/nam-ndss26.pdf"
doiurl: "https://doi.org/10.14722/ndss.2026.241857"
codeurl: "https://github.com/NetSP-KAIST/shield"
artifacturl: "https://zenodo.org/records/17490769"
bibtex: |
  @inproceedings{nam2026heracles,
    title = {{On the Security Risks of Memory Adaptation and Augmentation in Data-plane DoS Mitigation}},
    author = {Nam, Hocheol and Lim, Daehyun and Zhou, Huancheng and Gu, Guofei and Kang, Min Suk},
    booktitle = {Proceedings of the 2026 Network and Distributed System Security Symposium (NDSS'26)},
    pages = {1-20},
    year = {2026},
  }
---

Data-plane programmability in commodity switches is reshaping the landscape of denial-of-service (DoS) defense by enabling adaptive, line-rate mitigation strategies. Recent systems like Cerberus [SP'24] augment limited switch memory with control-plane support to rapidly respond to evolving attacks. In this paper, we reveal a subtle yet critical vulnerability in this model; that is, the very mechanisms that enable the defense system’s agility and scalability can be subverted by a new class of coordinated DoS attacks. We present Heracles, the first attack to exploit hardware-level constraints in programmable switches to orchestrate precise resource contention across dataplane and control-plane memory. By leveraging side-channel timing signals, Heracles triggers synchronized augmentation, memory squeezing, and time-window exploitation, which are three orthogonal contention strategies that significantly degrade or even completely disable the DoS mitigation capabilities. We implement and test Heracles against real Tofino hardware and show that it can reliably disrupt DoS defenses across diverse DoS attack profiles, even when using loosely (1–2 second) timesynchronized attack sources. To mitigate this threat, we propose Shield, a multi-layered DoS mitigation sketch architecture that decouples memory operations across control- and data-plane layers, effectively mitigating the Heracles attack while preserving both line-rate performance and detection accuracy.
