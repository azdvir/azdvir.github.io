---
layout: page
title: Encrypted Traffic Classification
description: Identifying applications and services from encrypted network flows using machine learning
img: assets/img/4.jpg
importance: 1
category: research
related_publications: false
---

Over 90% of internet traffic is now encrypted, rendering traditional port-based and payload-based classification methods obsolete. This project develops **machine learning frameworks for classifying encrypted network traffic** without any decryption.

We exploit the rich information available outside the payload:

- **Flow-level features**: packet sizes, inter-arrival times, byte distributions
- **TLS metadata**: handshake parameters, certificate chains, ALPN extensions
- **Graph representations**: connection graphs between hosts and services

Our work spans multiple application domains — video streaming, VoIP, cloud storage, social media — and addresses real-world challenges including imbalanced classes, concept drift, and zero-day application identification via few-shot learning.

The resulting classifiers are deployable in ISP-scale network monitoring, enterprise firewalls, and QoS policy enforcement systems.
