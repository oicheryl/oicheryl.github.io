---
layout: post
title: "Multi-Arch Infrastructure from the Ground up"
description: "Cheryl Hung discusses why companies are switching to Arm and tips for multi-arch cloud native infrastructure."
image: https://pbs.twimg.com/media/FuFRiLNWYAQPnkP?format=jpg&name=medium
location: Amsterdam, Netherlands
slides: //www.slideshare.net/slideshow/embed_code/key/bZHYONwQPPMZVZ
tags:
  - "2023"
  - Images
  - Slides
---

Love to see a full house at KubeCon CloudNativeCon EU in Amsterdam! Such a great crowd and great questions too.

At a high level, the goal of Multi-Arch infrastructure is that workloads can run on the best hardware for their price/performance needs, without developers being concerned with the underlying architecture. That doesn’t mean it’s easy! Multi-Arch touches Infra As Code, CI/CD, packaging, binaries, images, Kubernetes upgrades, testing, scheduling, rollout, reproducible builds, performance testing and more. This talk looks at how early adopters handled the challenges so you are prepared for the road ahead.

The biggest drivers for Multi-Arch infrastructure are reducing cloud costs and M1-based laptops. Migration is in three phases:
* Inform - inventory your software stack and check everything for Arm support
* Optimize - provision test environments for upgrading and testing
* Operate - update your K8s cluster and other infra, then roll out using canary or blue-green deployment
Case studies
* FusionAuth
* [The Present and Future of Arm and AWS Graviton at Honeycomb](https://www.honeycomb.io/blog/present-future-arm-aws-graviton-honeycomb)
