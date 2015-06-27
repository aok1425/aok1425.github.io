---
layout: post
title: ms-very-quietly-adds-18-new-trusted-root-certs
comments: true
---

Earlier this month, Microsoft has started silently pushing the following new root certificates to all supported Windows systems. The problem is, they did not announce or document this change in any KB article or advisory. Even worse: not even their official MCP (Microsoft Certificate Program) member list makes no mention of these changes.  As some of these new certificates relate to rather 'brutal' regimes (China, Tunisia), or completely unknown authorities (RXC-R2? Now what the hell is that? Both the name and thumbprint are totally unknown on the Web), color me very, very suspicious. 

Using my faithful <A HREF=http://www.wilderssecurity.com/threads/rcc-check-your-systems-trusted-root-certificate-store.373819/>RCC command-line scanner</A>, I quickly identified the following certificates: 

    * 0f36385b811a25c39b314e83cae9346670cc74b4: GDCA TrustAUTH R5 ROOT
    * 1b3d1114ea7a0f9558544195bf6b2582ab40ce9a: S-Trust Universal Root CA
    * 1f3f1486b531882802e87b624d420295a0fc721a: Notarius Root Certificate Authority
    * 22fdd0b7fda24e0dac492ca0aca67b6a1fe3f766: Certplus Root CA G1
    * 2c8affce966430ba04c04f81dd4b49c71b5b81a0: RXC-R2
    * 32f442093b36d7031b75ca4daddcb327faa02b9c: Swedish Government Root Authority v2
    * 3bc6dce00307bd676041ebd85970c62f8fda5109: CCA India 2015
    * 46af7a31b599460d469d6041145b13651df9170a: MULTICERT Root Certification Authority 01
    * 4f658e1fe906d82802e9544741c954255d69cc1a: Certplus Root CA G2
    * 6e2664f356bf3455bfd1933f7c01ded813da8aa6: OpenTrust Root CA G3
    * 795f8860c5ab7c3d92e6cbf48de145cd11ef600b: OpenTrust Root CA G2
    * 7991e834f7e2eedd08950152e9552d14e958d57e: OpenTrust Root CA G1
    * 8094640eb5a7a1ca119c1fddd59f810263a7fbd1: GlobalSign Root CA - R6
    * 9638633c9056ae8814a065d23bdc60a0ee702fa7: Tunisian Root Certificate Authority - TunRootCA2
    * a2b86b5a68d92819d9ce5dd6d7969a4968e11991: CCA India 2014
    * d27ad2beed94c0a13cc72521ea5d71be8119f32b: WoSign ECC
    * fbeddc9065b7272037bc550c9c56debbf27894e1: WoSign G2
 