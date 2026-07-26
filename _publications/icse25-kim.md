---
paper_key: kim_icse25
title: "Fork State-Aware Differential Fuzzing for Blockchain Consensus Implementations"
collection: publications
category: conferences
permalink: /publication/kim-icse25/
excerpt: "We introduce Forky, a fork state-aware differential fuzzing framework for finding semantic discrepancies in blockchain consensus implementations. We test Forky on Bitcoin and Ethereum, which are the representatives of the two major blockchain consensus algorithm families, PoW and PoS consensus algorithms."
date: 2025-04-27
venue: "IEEE/ACM International Conference on Software Engineering (ICSE)"
location: "Ottawa, ON, Canada"
abbr: "ICSE"
tier: "Tier-1"
detail_page: true
authors: "Wonhoi Kim<sup>*</sup>, **Hocheol Nam**<sup>*</sup>, Muoi Tran, Amin Jalilov, Zhenkai Liang, Sang Kil Cha, and Min Suk Kang"
paperurl: "/files/kim-icse25.pdf"
doiurl: "https://doi.org/10.1109/ICSE55347.2025.00085"
codeurl: "https://github.com/NetSP-KAIST/forky"
artifacturl: "https://zenodo.org/records/14641017"
additional_info: "<sup>*</sup>Co-first authors"
bibtex: |
  @inproceedings{kim2025fork,
    title = {{Fork State-Aware Differential Fuzzing for Blockchain Consensus Implementations}},
    author = {Wonhoi Kim and Hocheol Nam and Muoi Tran and Amin Jalilov and Zhenkai Liang and Sang Kil Cha and Min Suk Kang},
    booktitle = {Proceedings of the 47th IEEE/ACM International Conference on Software Engineering (ICSE'25)},
    pages = {3048-3059},
    year = {2025},
  }
---

Blockchain networks allow multiple client implementations of the same consensus algorithm by different developers to coexist in the same system. Ensuring correct implementations among these heterogeneous clients is crucial, as even slight semantic discrepancies in their implementations can lead to safety failures. While existing fuzzing frameworks have discovered implementation ﬂaws in blockchain, they suffer from several challenges in testing them with sequences of conﬂicting blocks, called forks. Existing tools fail to adequately assess the forkhandling processes in blockchain implementations when relying on traditional code coverage feedback, which lacks the granularity needed to navigate the diverse and complex fork-handling scenarios. This paper introduces Forky, a fork state-aware differential fuzzing framework designed to detect implementation discrepancies within the critical fork-handling process with its novel fork-aware mutation and fork-diversifying feedback mechanisms. We test Forky on the two most inﬂuential blockchain projects: Bitcoin and Ethereum, which are the representatives of the two major blockchain consensus algorithm families, Proof-of-Work (PoW) and Proof-of-Stake (PoS) consensus algorithms.
