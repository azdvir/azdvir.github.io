---
layout: page
title: Encrypted QoE Classification
description: Inferring video streaming quality of experience from encrypted adaptive bitrate traffic
img: assets/img/5.jpg
importance: 5
category: research
related_publications: false
---

Streaming platforms like Netflix, YouTube, and Disney+ use **HTTP Adaptive Streaming (HAS)** to dynamically adjust video quality to network conditions. For ISPs and network operators, understanding the quality users actually experience — without decrypting HTTPS traffic — is a critical but unsolved challenge.

This project develops techniques to **infer Quality of Experience (QoE) metrics directly from encrypted HAS traffic**:

- **Bitrate estimation**: identifying video resolution segments from encrypted flow patterns
- **Stall detection**: recognizing rebuffering events from throughput signatures  
- **Quality prediction**: mapping network-layer observations to user-perceived MOS scores

We address the complexity introduced by CDN multi-pathing, QUIC transport, and per-title encoding, building robust models that generalize across streaming providers and network environments.

Our research enables network operators to enforce QoE-driven SLAs and proactively optimize streaming performance — all without compromising user privacy.
