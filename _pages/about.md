---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I’m a Ph.D. candidate in Computer Science (Information Security Program) at [KAIST](https://www.kaist.ac.kr), where I am a member of the [Network Security and Privacy Research Lab](https://netsp.kaist.ac.kr) advised by Prof. [Min Suk Kang](https://netsp.kaist.ac.kr/min-suk-kang). I received my B.S. in Software Science at Dankook University, and I completed compulsory military service at the Capital Defense Command, R.O.K. Army. My current research interests are:
+ Network security including:
  - Network attack (e.g., Botnets, DDoS) prevention, detection, and response;
  - Security for emerging networks (e.g., SDN, Programmable data-plane);
  - Mobile and wireless network security;
  - Space and satellite communication security; and
+ Security and privacy for blockchains and cryptocurrencies.

## News

{% include news-list.html limit=10 compact=true %}

<p class="news__more"><a href="{{ '/news/' | relative_url }}">View all news <span aria-hidden="true">&rarr;</span></a></p>

---

## Selected Publications

{% include selected-publications.html keys=site.data.selected_publications %}
