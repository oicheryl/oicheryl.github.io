---
layout: post
title: "Cloud Native London November 2026: Pluto, DLM Capital Group, and Truelayer"
description: "Speakers from Pluto, DLM Capital Group, and Truelayer join us at the Cloud Native London meetup November 2026, hosted by Cheryl Hung"
location: London, UK
image: /images/2026-11-04-cloud-native-london-november-2026.jpeg
video: https://www.youtube.com/embed/vDRvRdX6GWU
tags:
  - Photos
  - Video
  - Meetup
  - "2026"
---

Three speakers from Pluto, DLM Capital Group, and Truelayer joined us at the November Cloud Native London meetup at the Just Eat office, as well as via the YouTube/LinkedIn livestreams. 

We are immensely grateful to [Cloudsmith](https://cloudsmith.com), and [TechShack](https://www.tech-shack.co/) for their generous support and sponsorship. 

### Overview
Kicking off our evening was Ace Vinayak from Pluto discussing [Admission Control for AI Coding Agents: Fail-Closed Policy on Every Tool Call](https://www.youtube.com/live/vDRvRdX6GWU?si=_Mxmgtg1Tdv9fxqe&t=1369)(starting at 22:49). His takeaways suggested:
* Admission-control agent tool calls the same way you'd admission-control a cluster. Turn each call into facts (the command, what it touches, which environment) and decide it against written policy before it runs. The check should be deterministic, not one LLM reviewing another.	
* Fail closed on anything the gate can't understand. Agents find the gaps: wrapped shells, chained commands, scripts written and then run. If a call can't be fully parsed, the gate blocks it or asks a human. It never lets it through.	
* Tier decisions and treat policy as code. Allow / ask / block tiers keep humans in the loop only where the risk is real, so approvals don't turn into rubber-stamping. Keep policies in version control with regression tests, and turn every bypass you find into a new test case.

Following this was Pereowei Daniel from DLM Capital Group explaining that [Kubernetes Is Not Your Hyperledger Fabric Control Plane](https://www.youtube.com/live/vDRvRdX6GWU?si=ijtsyRw6v0Daz1ty&t=3229)(starting at 53:49). His takeaways mentioned that:
* Kubernetes workload health is not Fabric readiness. A peer can be running while still lacking the correct identity, channel membership, chaincode definition, or usable service path.
* Production Fabric operations benefit from a declarative, reconciliation-driven model. Desired state gives teams a clearer way to manage repeatable changes, recover from partial failure, and observe progress.
* Multi-organization Fabric networks need explicit ownership boundaries. Per-organization namespaces, independently managed infrastructure, and federated joining are foundational for realistic production deployments.
Check out [his slides here](Kubernetes Is Not Your Hyperledger Fabric Control Plane — Cloud Native London.pptx)

And wrapping up our evening, we had Surya Pandian from Truelayer describing [RabbitMQ cluster migration](https://www.youtube.com/live/vDRvRdX6GWU?si=Ywfwd4au69GX3p5C&t=5908)(starting at 1:38:28). She explored how:
*”helpful” retry logic is what turns a blip into an outage.
During an incident, consumers that nack-and-requeue on a publish timeout hand the message straight back to the head of the queue. The broker never gets a chance to recover, and duplicates pile up. The retry that was meant to help becomes the load that keeps the incident alive. Test failure behaviour under broker stress, not just app logic."	
* A platform migration is a people problem first.
The hard part wasn't the migration. It was coordinating many teams, each with its own services and priorities. 
What worked:
One support channel for questions.
Automated checks so every team could see its own progress.
A small squad owning the plan and playbooks.
Library maintainers making the safe path the default.
* We stand on open source, and AI helps us give back.
The whole stack rests on open source: RabbitMQ itself, the Rust AMQP client lapin, Kubernetes and the tooling around them. When our Rust libraries wouldn't reconnect after broker maintenance, the real fix was in the upstream client, not in workarounds in our own code. We fixed it there first and then rolled it out, so every service benefited, and so does anyone else using the library.
Contributing upstream used to be a big cost. You had to understand an unfamiliar codebase, its conventions and its test setup, and you had to write a change the maintainers would accept. AI lowers that barrier:
It explains unfamiliar code and the project's conventions.
It drafts tests, PR descriptions and documentation.
It helps you reproduce a bug and narrow it down.

And of course, our usual group photo!
![](/images/2026-11-04-cloud-native-london-november-2026.jpeg)

###Quick news: we're changing our name!

Cloud Native London is now ***AI & Cloud London***.

Since 2017, we've run over 100 events and built a community of 10,000+ engineers. Cloud native is now the baseline for how everyone builds, and a lot of our conversations are about AI. I wanted the name to match what we're all talking about.

It should also help newcomers find us more easily, and give speakers and sponsors a simpler way to pitch us internally.

The good news is that nothing else changes. Same format, same friendly crowd, same great talks and chats over pizza and drinks. Thanks for being part of this fantastic community, and I’ll see you at our December meetup!

### AI & Cloud London December

Our next meetup will be on Wednesday 2nd December, when we'll be joined by speakers from HAProxy Technologies, meshcloud, and AudioStack! [RSVP and save the date now!](https://www.meetup.com/cloud-native-london/events/316265226/). 

I’ll see you next month. Stay safe, stay healthy, and see you soon!

Cheryl (@oicheryl) 
