---
layout: post
title: "Cloud Native London October 2025: Apple, Container Solutions, and ScaleOps"
description: "Speakers from Apple, Container Solutions, and ScaleOps join us at the Cloud Native London meetup October 2025, hosted by Cheryl Hung"
location: London, UK
image: /images/2025-10-01-cloud-native-london-october-2025.jpeg
video: https://www.youtube.com/embed/zjOmbeU1fhY
tags:
  - Photos
  - Video
  - Meetup
  - "2025"
---

Three speakers from Apple, Container Solutions, and ScaleOps joined us at the October Cloud Native London meetup at Container Solutions, as well as via the YouTube/Twitch livestreams. 

We are immensely grateful to [Testkube](https://testkube.io/), [TechShack](https://www.tech-shack.co/), [Swift](https://developer.apple.com/swift/), and [Sidero](http://siderolabs.com/) for their generous support and sponsorship. More info on them below!

### Overview
Kicking off our evening was Euan Harris from Apple talking about [How To Put Swift in a Box: Container Images From Scratch With Swift Container Plugin](https://www.youtube.com/live/zjOmbeU1fhY?si=-JMD6n-GQ8Xu9F4S&t=928)(starting at 15:28). He explained:
* Did you know that you can build a container image without using a container runtime?   [swift-container-plugin](https://github.com/apple/swift-container-plugin) is a plugin for Swift Package Manager, Swift's native build system, which takes care of packaging your executable in a container image and publishing it to a registry.
* Of course, the executable needs to be able to run on your deployment platform.   For that you can lean on Swift's excellent cross-compilation support and use a [Swift SDK](https://www.swift.org/documentation/articles/static-linux-getting-started.html) to cross-compile to Linux, even across different processor architectures.
* You can deploy your image on any standards-compliant container runtime, but if you're a macOS user take a look at `container` [https://github.com/apple/container](https://github.com/apple/container).   It's a new, open-source container runtime specifically built to run Linux-based container images easily and efficiently on macOS.
*While you're there, also check out the new open-source `containerization` framework [https://github.com/apple/containerization](https://github.com/apple/containerization).   `container` is built on top of it, and it's designed to let you build your own container tools and add container-related features to your projects.

Following this, Chris Vermeulen from Container Solutions explained [Compliance for Dummies: A Primer for a Compliance-Minded Future](https://www.youtube.com/live/zjOmbeU1fhY?si=FDACAQeVQYdqIo2e&t=4109)(starting at 1:08:29). He discussed: 
* What compliance is, and some key terms which are important to know
* How the industry is embracing standardised formats, to allow more automatability and interoperability for compliance reporting and tracking
* How tools like The Continuous Compliance Framework are utilising these new standards to build the next generation of cloud native tooling for a compliance minded future.

And wrapping up our evening was Nic Vermande, ScaleOps describing [Smoke, Mirrors, and Metrics: A Kernel Detective's Guide to Cluster Resource Scaling](https://www.youtube.com/live/zjOmbeU1fhY?si=3mBGh8bxYfcHRhyw&t=5818)(starting at 1:36:58). His takeaways are about how to:
* Gain a practical framework for orchestrating HPA, VPA, and KEDA together, turning reactive chaos into predictable resource management	
* Understand how the Kubernetes metrics pipeline distorts kernel reality.	
* Explore how to use kernel data to align autoscalers for stable, efficient scaling.

And of course, our usual group photo!
![](/images/2025-10-01-cloud-native-london-october-2025.jpeg)

With many thanks to our sponsors this month:

[Testkube](https://testkube.io/) powers cloud-native continuous testing that scales with your team and keeps up with AI-driven release velocity.

[TechShack](https://www.tech-shack.co/) are a tech recruitment agency specialising in the Cloud, Engineering and AI. TechShack exists to build high-performing tech teams by putting community, connection, and quality first.

[Swift](https://developer.apple.com/swift/) is an open source general purpose programming language, recognized by world security organizations for its memory safety; its performance and beautiful syntax make it a great option for the cloud native space. Try it out and talk to us on [forums.swift.org](forums.swift.org).

[Sidero](http://siderolabs.com/), the builders of Talos Linux and Omni, creates an easier way to run Kubernetes. Talos Linux and Omni bring simplicity and security to edge, data center, bare metal, and hybrid Kubernetes. By delivering scalable management for Kubernetes clusters, infrastructures are secure by default, easy to use, and reliable to operate.

## Cloud Native London November

Our next meetup will be on Wednesday 1st October, when we'll be joined by speakers from FusionAuth, Cast AI, and Meghdo! [RSVP and save the date now!](https://www.meetup.com/cloud-native-london/events/310408493/). 

Stay safe, stay healthy, and see you in a month!

Cheryl (@oicheryl) 
