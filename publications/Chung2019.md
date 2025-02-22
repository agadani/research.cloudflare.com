---
title: "RPKI is coming of age: A longitudinal study of RPKI deployment and invalid route origins"
year: 2019
location: Proceedings of the Internet Measurement Conference, pp. 406-419. 2019.
authors:
  - Taejoong Chung
  - Emile Aben
  - Tim Bruijnzeels
  - Balakrishnan Chandrasekaran
  - David Choffnes
  - Dave Levin
  - Bruce M. Maggs
  - Alan Mislove
  - Roland van Rijswijk-Deij
  - John Rula
  - nick-sullivan
url: https://dl.acm.org/doi/pdf/10.1145/3355369.3355596
doi: 10.1145/3355369.3355596
related_areas:
  - measurement
  - security
---

Despite its critical role in Internet connectivity, the Border Gateway Protocol (BGP) remains highly vulnerable to attacks such as prefix hijacking, where an Autonomous System (AS) announces routes for IP space it does not control. To address this issue, the Resource Public Key Infrastructure (RPKI) was developed starting in 2008, with deployment beginning in 2011. This paper performs the first comprehensive, longitudinal study of the deployment, coverage, and quality of RPKI.

We use a unique dataset containing all RPKI Route Origin Authorizations (ROAs) from the moment RPKI was first deployed, more than 8 years ago. We combine this dataset with BGP announcements from more than 3,300 BGP collectors worldwide. Our analysis shows the after a gradual start, RPKI has seen a rapid increase in adoption over the past two years. We also show that although misconfigurations were rampant when RPKI was first deployed (causing many announcements to appear as invalid) they are quite rare today. We develop a taxonomy of invalid RPKI announcements, then quantify their prevalence. We further identify suspicious announcements indicative of prefix hijacking and present case studies of likely hijacks.

Overall, we conclude that while misconfigurations still do occur, RPKI is "ready for the big screen," and routing security can be increased by dropping invalid announcements. To foster reproducibility and further studies, we release all RPKI data and the tools we used to analyze it into the public domain.
