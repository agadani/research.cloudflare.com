---
title: Is the web ready for OSCP must-staple?
year: 2018
location: Proceedings of the Internet Measurement Conference 2018, pp. 105-118. 2018.
authors:
  - Taejoong Chung
  - Jay Lok
  - Balakrishnan Chandrasekaran
  - David Choffnes
  - Dave Levin
  - Bruce M. Maggs
  - Alan Mislove
  - John Rula
  - nick-sullivan
  - Christo Wilson
url: https://dl.acm.org/doi/abs/10.1145/3278532.3278543
doi: 10.1145/3278532.3278543
related_areas:
  - measurement
  - security
---

TLS, the de facto standard protocol for securing communications over the Internet, relies on a hierarchy of certificates that bind names to public keys. Naturally, ensuring that the communicating parties are using only valid certificates is a necessary first step in order to benefit from the security of TLS. To this end, most certificates and clients support OCSP, a protocol for querying a certificate's revocation status and confirming that it is still valid. Unfortunately, however, OCSP has been criticized for its slow performance, unreliability, soft-failures, and privacy issues. To address these issues, the OCSP Must-Staple certificate extension was introduced, which requires web servers to provide OCSP responses to clients during the TLS handshake, making revocation checks low-cost for clients. Whether all of the players in the web's PKI are ready to support OCSP Must-Staple, however, remains still an open question.

In this paper, we take a broad look at the web's PKI and determine if all components involved --- namely, certificate authorities, web server administrators, and web browsers --- are ready to support OCSP Must-Staple. We find that each component does not yet fully support OCSP Must-Staple: OCSP responders are still not fully reliable, and most major web browsers and web server implementations do not fully support OCSP Must-Staple. On the bright side, only a few players need to take action to make it possible for web server administrators to begin relying on certificates with OCSP Must-Staple. Thus, we believe a much wider deployment of OCSP Must-Staple is an realistic and achievable goal.
