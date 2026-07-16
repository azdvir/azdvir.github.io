---
layout: page
title: Encrypted Traffic Classification
description: Identifying applications and services from encrypted network flows using machine learning
img: assets/img/4.jpg
importance: 1
category: research
related_publications: false
---

Over 90% of internet traffic is now encrypted, rendering traditional classification methods obsolete. This project develops ML frameworks for classifying encrypted network traffic without decryption.

We exploit rich information outside the payload: flow-level features (packet sizes, inter-arrival times), TLS metadata (handshake parameters, certificate chains), and graph representations of communication patterns.

Our work spans video streaming, VoIP, cloud storage, and social media — addressing concept drift, imbalanced classes, and zero-day identification via few-shot learning.
