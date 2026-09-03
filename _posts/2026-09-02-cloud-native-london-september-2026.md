---
layout: post
title: "Cloud Native London September 2026: HAProxy Technologies, Mia-Platform, and DLM Capital Group"
description: "Speakers from HAProxy Technologies, Mia-Platform, and DLM Capital Group join us at the Cloud Native London meetup September 2026, hosted by Cheryl Hung"
location: London, UK
image: /images/2026-09-02-cloud-native-london-september-2026.jpeg
video: https://www.youtube.com/embed/UfxSQ9aA4Vc
tags:
  - Photos
  - Video
  - Meetup
  - "2026"
---

Three speakers from HAProxy Technologies, Mia-Platform, and DLM Capital Group joined us at the September Cloud Native London meetup at the Just Eat office, as well as via the YouTube/LinkedIn livestreams. 

We are immensely grateful to [HAProxy Technologies](https://www.haproxy.com), [Mia-Platform](https://mia-platform.eu), [Chronosphere, a Palo Alto Networks company](https://chronosphere.io/), [cloudsmith](https://cloudsmith.com), and [TechShack](https://www.tech-shack.co/) for their generous support and sponsorship. 

### Overview
Kicking off our evening was Baptiste Assmann from HAProxy Technologies discussing [AI Inference Routing: Sovereign Control for Your AI Factory](https://www.youtube.com/live/UfxSQ9aA4Vc?si=RKBpDo0Ohd4CxqMt&t=1146)(starting at 19:06). His takeaways explained that:
* Why inference traffic behaves unlike anything else you route: how prompt size, prefill and decode phases, and whether the target model is already loaded reshape request duration, connection lifetime and server load, and why the default algorithm choices work against you.
* The HAProxy rules that answer each of those behaviours: routing on the model name in the request body, health checks that verify the model is actually loaded rather than the process is alive, streaming responses without buffering or mid-stream timeouts, and retry and timeout settings that suit a sixty-second request.
* You can run this yourself: the whole configuration is open source and copyable, and every prompt, model input and inference response stays inside your own infrastructure.

And wrapping up our evening, we had Giulio Roggero from Mia-Platform explaining his thoughts behind [Telemetry for the Mind: AI Agent Observability & DORA-Driven Scoring](https://www.youtube.com/live/UfxSQ9aA4Vc?si=pZvKzWhjKhAOY2Yn&t=3072)(starting at 51:12). He explained that:
* AI Agents are Microservices—Treat Them Like It: 
Moving from single-prompt LLM calls to multi-step agentic workflows means managing state machines, tool invocations, and execution loops. We need to stop treating agents like black boxes and start applying cloud-native standards. By instrumenting agent sessions with OpenTelemetry, you gain distributed visibility into prompt flows, tool latency, and token consumption just like you would for any API call in a microservice architecture.
* DORA Metrics Aren't Just for Deployment—They Work for Agentic Scoring: 
Evaluating an agent isn't binary; a response can be partially correct while still burning through unnecessary tokens or retries. Adapting classic DORA metrics (like Lead Time, Change Failure Rate, and Mean Time to Recovery) into a weighted scoring framework provides an operational baseline. This lets engineering teams measure session health, pinpoint structural bottlenecks, and calculate true ROI.
* Close the Loop with "Evaluator LLMs" for Automated Healing: 
Observability is only half the battle; real-time resolution is the ultimate goal. By feeding OpenTelemetry bottleneck data into a specialized Evaluator LLM, system architectures can automatically diagnose failed session loops and generate targeted prompt patches or tool adjustments—shifting your agentic platform from reactive debugging to self-improving infrastructure.

Unfortunately we had some technical issues which prevented our third speaker from giving his talk - hopefully we will be able to bring him back another time, watch this space! 

And of course, our usual group photo!
![](/images/2026-09-02-cloud-native-london-september-2026.jpeg)

## Cloud Native London October

Our next meetup will be on Wednesday 7th October, when we'll be joined by speakers from Testkube, MongoDB, and Cisco! [RSVP and save the date now!](https://www.meetup.com/cloud-native-london/events/314662668/). 

I’ll see you next month. Stay safe, stay healthy, and see you soon!

Cheryl (@oicheryl) 
