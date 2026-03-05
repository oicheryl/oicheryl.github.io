---
layout: post
title: "Cloud Native London March 2026: Aerospike, HAProxy  Technologies, and more"
description: "Speakers from Aerospike, HAProxy Technologies, and more join us at the Cloud Native London meetup March 2026, hosted by Cheryl Hung"
location: London, UK
image: /images/2026-03-04-cloud-native-london-march-2026.jpeg
video: https://www.youtube.com/embed/JLnNKaTEeYY
tags:
  - Photos
  - Video
  - Meetup
  - "2026"
---

Three speakers from Aerospike, HAProxy Technologies, and more joined us at the March Cloud Native London meetup at the fabulous Thought Machine event space, as well as via the YouTube/LinkedIn livestreams. 

We are immensely grateful to [Aerospike](https://aerospike.com/), [HAProxy Technologies](https://www.haproxy.com/), and [TechShack](https://www.tech-shack.co/) for their generous support and sponsorship. 

### Overview
Kicking off our evening was Behrad Babaee from Aerospike discussing [Predictable Systems in an Unpredictable World](https://www.youtube.com/live/JLnNKaTEeYY?si=08beWYlgjcWSeqBx&t=1304)(starting at 21:44). His takeaways explained that:
* Average performance and even P99 are misleading; what truly defines your system is its behaviour at the extreme tail when conditions deteriorate.
* The assumptions systems are built upon are almost always quietly eroding.
* Predictability must be treated as a first-class property of a system.

Following this, we had Baptiste Assmann from HAProxy Technologies describing [Observability with HAProxy: detecting what is not working and why](https://www.youtube.com/live/JLnNKaTEeYY?si=OgVm-XEajN5eDVH6&t=3143)(starting at 52:23). He mentioned that:
* __The load balancer is your best source of truth.__ Because HAProxy sits between the client and the server, it maintains two distinct connections. This allows it to act as an "observation tower," providing impartial data on network retransmits, application processing times, and client bandwidth limitations that other components cannot see.
* __Timers are critical for root cause analysis.__ High-level monitoring averages often hide the root cause. By analyzing HAProxy's internal timers—specifically Queue time (Tq), Connect time (Tc), and Response time (Tr)—you can mathematically determine if latency is caused by a saturated server, a network packet loss, or a slow application query.
* __Observability reduces troubleshooting time.__ Detailed logging and termination codes allow you to move from "users are complaining" to identifying the exact source of the error (e.g., a specific server or a broken switch). While HAProxy may not fix a broken application, it drastically reduces the time required to isolate the issue so the right team can fix it.

And wrapping up our evening was Alam Ahmed exploring [eBPF: Revolutionizing Cloud-Native Security](https://www.youtube.com/live/JLnNKaTEeYY?si=AZqLSMtf9ubU3A6s&t=6047)(starting at 1:40:47). He described how:
* Traditional security tools are architecturally misaligned with cloud-native systems—they assume static IPs and persistent hosts while containers spin up/down in seconds, creating dangerous blind spots that delay 67% of deployments and miss kernel-level attacks entirely.	
* eBPF enables kernel-native security with 10x performance gains—by executing sandboxed programs directly in the Linux kernel with JIT compilation, it eliminates context-switching overhead (<1% CPU impact), requires zero code changes, and provides complete container/Kubernetes context for every event.	
* Production-proven tools are available now—the CNCF eBPF ecosystem grew 4.5x to 41+ projects in two years, with graduated projects like Falco (runtime threat detection), Tetragon (kernel-level enforcement), and Cilium (network security) already securing hyperscale infrastructure at Meta, Google, and billions of Android devices.

And of course, our usual group photo!
![](/images/2026-03-04-cloud-native-london-march-2026.jpeg)

## Cloud Native London April

Our next meetup will be on Wednesday 1st April, when we'll be joined by speakers from Cloudsmith, Testkube, and Diagrid! [RSVP and save the date now!](https://www.meetup.com/cloud-native-london/events/312772371/). 

Stay safe, stay healthy, and see you in a month!

Cheryl (@oicheryl) 
