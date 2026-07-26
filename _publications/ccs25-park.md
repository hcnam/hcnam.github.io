---
paper_key: park_ccs25
title: "On Frontrunning Risks in Batch-Order Fair Systems for Blockchains"
collection: publications
category: conferences
permalink: /publication/park-ccs25/
excerpt: "We examine frontrunning risks in batch-order fair blockchain systems (like Themis [CCS'23]) and propose the 'Ambush attack' that enables frontrunning attacks that remain possible despite fair-ordering guarantees."
date: 2025-10-13
venue: "ACM SIGSAC Conference on Computer and Communications Security (CCS)"
location: "Taipei, Taiwan"
abbr: "CCS"
tier: "Tier-1"
detail_page: true
authors: "Eunchan Park, Taeung Yoon, **Hocheol Nam**, Deepak Maram, and Min Suk Kang"
paperurl: "/files/park-ccs25.pdf"
doiurl: "https://doi.org/10.1145/3719027.3744879"
codeurl: "https://github.com/NetSP-KAIST/the-ambush-attack"
fullversionurl: "https://eprint.iacr.org/2025/1168"
artifacturl: "https://zenodo.org/records/15703035"
bibtex: |
  @inproceedings{park2025frontrunning,
    title = {{On Frontrunning Risks in Batch-Order Fair Systems for Blockchains}},
    author={Park, Eunchan and Yoon, Taeung and Nam, Hocheol and Maram, Deepak and Kang, Min Suk},
    booktitle = {Proceedings of the 32nd ACM Conference on Computer and Communications Security (CCS)},
    year = {2025},
  }
---

In timing-sensitive blockchain applications, such as decentralized finance (DeFi), achieving first-come-first-served (FCFS) transaction ordering among decentralized nodes is critical to prevent frontrunning attacks. Themis [CCS'23], a state-of-the-art decentralized FCFS ordering system, has become a key reference point for highthroughput fair ordering systems for real-world blockchain applications, such as rollup chains and decentralized sequencing, and has influenced the design of several subsequent proposals. In this paper, we critically analyze its core system property of practical batch-order fairness and evaluate the frontrunning resistance claim of Themis. We present the Ambush attack, a new frontrunning technique that achieves nearly 100% success against the practical batch-order fair system with only a single malicious node and negligible attack costs. This attack causes a subtle temporary information asymmetry among nodes, which is allowed due to the heavily optimized communication model of the system. A fundamental trade-off we identify is a challenge in balancing security and performance in these systems; namely, enforcing timely dissemination of transaction information among nodes (to mitigate frontrunning) can easily lead to non-negligible network overheads (thus, degrading overall throughput performance). We show that it is yet possible to balance these two by delaying transaction dissemination to a certain tolerable level for frontrunning mitigation while maintaining high throughput. Our evaluation demonstrates that the proposed delayed gossiping mechanism can be seamlessly integrated into existing systems with only minimal changes.
