---
layout: post
title: "Cloud Native London May 2026: Pulumi, Oligo Security, and Cloud Combinator"
description: "Speakers from Pulumi, Oligo Security, and Cloud Combinator join us at the Cloud Native London meetup May 2026, hosted by Cheryl Hung"
location: London, UK
image: /images/2026-05-06-cloud-native-london-may-2026.jpeg
video: https://www.youtube.com/embed/9zZP5uwFuUE
tags:
  - Photos
  - Video
  - Meetup
  - "2026"
---

Three speakers from Pulumi, Oligo Security, and Cloud Combinator joined us at the May Cloud Native London meetup at the beautiful Vorboss offices, as well as via the YouTube/LinkedIn livestreams. 

We are immensely grateful to [Pulumi](https://www.pulumi.com/), [Oligo Security](https://www.oligo.security/), and [TechShack](https://www.tech-shack.co/) for their generous support and sponsorship. 

### Overview
Kicking off our evening was Alberto Pose from Pulumi discussing [The End of Handoffs: Build, Run, Own in One Flow](https://www.youtube.com/live/9zZP5uwFuUE?si=tvPJwS-OP0XWTKdR&t=1027)(starting at 17:07). His takeaways explained that:
* Accountability must follow the work. As AI enables more people to make technical changes, responsibility can’t be separated. You build it, you run it, you own it - all the way to production. The goal is shared ownership of outcomes across dev and product.
* Tooling hasn’t caught up with AI speed. Code review and testing were built for human pace. With AI generating far more code, accountability alone doesn’t scale - without better tooling, it becomes overload.
* Old workflows break under AI. Traditional handovers and unwritten processes worked at human speed. With AI, higher failure rates and less predictability expose gaps quickly, making those workflows no longer reliable.

Following this, we had Idan Elor from Oligo Security explaining that [You Can’t Patch Fast Enough: What AI-Driven Attacks Mean](https://www.youtube.com/live/9zZP5uwFuUE?si=oRbC5qGl6gLSsmQN&t=2600)(starting at 43:20). He mentioned that:
* The window between vulnerability and exploitation is disappearing: AI is compressing the timeline from discovery to attack. What used to take weeks or months can now happen at unprecedented rates. This means organizations are increasingly exposed to vulnerabilities before they even know they exist, let alone have time to patch them.	
* Patching is necessary but no longer sufficient: Patching remains critical, but it’s no longer a reliable first line of defense. The scale and speed of modern attacks mean that security teams can’t depend on remediation cycles alone. In many cases, exploitation happens before patches are available or applied.	
* Security is shifting from vulnerabilities to behavior:  Instead of chasing an ever-growing list of CVEs, security teams need to focus on how exploits actually work. By understanding and blocking common exploit techniques, organizations can stop entire classes of attacks in real time, including zero-days.

And wrapping up our evening was Anton Nazaruk from Cloud Combinator describing [From Zero to HyperPod: Distributed Model Training on AWS](https://www.youtube.com/live/9zZP5uwFuUE?si=85AJKc9xdwkHcB3c&t=5414)(starting at 1:30:14). He described how:
* GPU workloads aren't like regular cloud-native apps. Capacity is genuinely scarce, failures at scale are expensive (you can lose hours of compute), and costs compound quickly. Treat GPU infrastructure as its own discipline.	
* Match the service to the shape of the work. Short runs with simple setup → SageMaker Training Jobs. Long, resilient training runs where losing days of progress would hurt → HyperPod. Want full control and willing to manage the infra yourself → EC2. The mistake is picking based on familiarity rather than fit.	
* The blueprint is four layers, not one. Compute (GPUs placed close together), network (fast enough for collectives), storage (hot path for checkpoints + durable path for datasets), and observability (training metrics, not just infra metrics). Get these right and scaling up becomes changing numbers, not rewriting architecture.

And of course, our usual group photo!
![](/images/2026-05-06-cloud-native-london-may-2026.jpeg)

## Cloud Native London June

Our next meetup will be on Wednesday 3rd June, when we'll be joined by speakers from HAProxy Technologies, WSO2, and Magentic! [RSVP and save the date now!](https://www.meetup.com/cloud-native-london/events/312972430/). 

Stay safe, stay healthy, and see you in a month!

Cheryl (@oicheryl) 
