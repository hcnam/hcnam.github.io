---
paper_key: baek_fc22
title: "Short Paper: On the Claims of Weak Block Synchronization in Bitcoin"
collection: publications
category: conferences
permalink: /publication/baek-fc22/
date: 2022-05-01
venue: "Financial Cryptography and Data Security (FC)"
excerpt: "We re-evaluates claims that Bitcoin has slow block propagation. We show that block synchronization is actually fast enough, and that previous slow-propagation claims stemmed from bugs and limits in monitoring tools. We finally ask several open-ended questions regarding the technical and ethical issues around monitoring blockchain networks."
location: "St. George's, Grenada"
abbr: "FC"
tier: "Tier-2"
detail_page: true
authors: "Seungjin Baek<sup>*</sup>, **Hocheol Nam**<sup>*</sup>, Yongwoo Oh, Muoi Tran, and Min Suk Kang"
paperurl: "https://fc22.ifca.ai/preproceedings/183.pdf"
doiurl: "https://doi.org/10.1007/978-3-031-18283-9_33"
preprinturl: "https://eprint.iacr.org/2021/1282"
additional_info: "<sup>*</sup>Co-first authors"
bibtex: |
  @inproceedings{baek2022short,
    title={{Short paper: On the claims of weak block synchronization in Bitcoin}},
    author={Baek, Seungjin and Nam, Hocheol and Oh, Yongwoo and Tran, Muoi and Kang, Min Suk},
    booktitle={International Conference on Financial Cryptography and Data Security (FC)},
    pages={663--671},
    year={2022},
    organization={Springer}
  }
---

Recent Bitcoin attacks [ICDCS'19, CCS'21a, CCS'21b] commonly exploit the phenomenon of so-called weak block synchronization in Bitcoin. The attacks use two independently-operated Bitcoin monitors— i.e., Bitnodes and a system of customized supernodes— to confirm that block propagation in Bitcoin is surprisingly slow. In particular, Bitnodes constantly reports that around 30% of nodes are 3 blocks (or more) behind the blockchain tip and the supernodes show that on average more than 60% of nodes do not receive the latest block even after waiting for 10 minutes. In this paper, we carefully re-evaluate these controversial claims with our own experiments in the live Bitcoin network and show that block propagation in Bitcoin is, in fact, fast enough (e.g., most peers we monitor receive new blocks in about 4 seconds) for its safety property. We identify several limitations and bugs of the two monitors, which have led to these inaccurate claims about the Bitcoin block synchronization. We finally ask several open-ended questions regarding the technical and ethical issues around monitoring blockchain networks.