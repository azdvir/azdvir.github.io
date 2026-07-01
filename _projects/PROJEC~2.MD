---
layout: page
title: Encrypted Malware Traffic Classification
description: Detecting malicious software through behavioral patterns in encrypted communications
img: assets/img/2.jpg
importance: 2
category: research
related_publications: false
---

As encryption becomes ubiquitous, traditional signature-based malware detection fails — malicious traffic hides behind TLS/HTTPS just like legitimate traffic. This project tackles the challenge of **classifying malware families directly from encrypted network flows**.

Rather than decrypting traffic (which is privacy-invasive and often infeasible), we extract behavioral and statistical features from:

- **TLS handshake metadata** (cipher suites, certificate fields, SNI)
- **Flow-level statistics** (packet size distributions, inter-arrival times)
- **Graph-based representations** of communication patterns

Using deep learning and graph neural networks, our classifiers achieve high accuracy in distinguishing malware families — ransomware, botnets, spyware — from benign encrypted traffic, enabling real-time threat response without compromising user privacy.
