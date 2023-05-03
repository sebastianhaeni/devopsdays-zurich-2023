# Day 1

Summarizes day 1 of the DevOpsDays Zurich 2023.

## Keynote-Speaker

__Topic__: Building High-Performing Teams: The crucial Role of Psychological Safety

__Takeaways__:

- "It's okay to fail" is the baseline. Having a Fail Fest is on the other end of the spectrum
- "Yes, and ..." - have open conversations
- Everyone is looking out for others to improve and get better at what they do. Leads to Growth acceleration.

Summary:

- Psychological safety is the foundation for innovative, efficient and fun teams
- Remember: we are all just mammals with a sensitive nervous system
- And this is what helps us feel safe:
  - Failure = ok
  - Have open conversations
  - Be willing to help
  - Embrace diversity, equity & inclusion

__New Tools__:

- https://my.manualof.me/


## Talk 1

__Topic__: Reporting on Reliability - Improving stakeholder conversations

__Takeaways__:

- The goal is not 100% uptime.
- Incident steps
  - What the heck?! => Incident status
  - What was that? => Postmortem
  - How's it going? => Periodic reviews

__Real-time incident managemenet__:

- Use chat
- Use live document (i.e. Google Docs)
- External people read the chat & doc, they don't ask questions
- People can offer help, but the response team first has to ack' for them to start helping

__Periodic Reviews__:

- Don't focus on incident counts. Each incident is unique
- Do focus on aggregated impact of incidents
  - Revenue lost
  - Error budget burned
  - Blast radius
  - Teams/Services affected
  - Look for patterns
- Look back: Team health
  - People: Does the team have the right mix of skills? What training can we offer?
  - Cognitive load: Is the team at capacity, or can they onboard additional services?
  - Toil: Are we doing the right amount? Are we learning from it?
  - Interrupts: Consder a paging "budget", (e.g. max 2 per on-call shift)
  - Morale: A happy team is a reliable team

__Look ahead__:

- Forecast demand
  - What capacity will be needed?
  - What other factors will become relevant?
- Forecast: work to be done
  - What's in the reliability backlog? What might prevent it from getting prioritized?
- Plans
  - Are stakeholders expecting improved reliability? Can we achieve it?
  - What launches are coming, for this team or related teams?
  - What known future bottlenecks/deprecations/etc can we prepare for?
  - How does the team's work align to (ongoing or emerging) organizational strategy?

## Talk 2

__Topic__: From a Backend Developer to DevOps - THE FORCE AWAKENS

__Takeaways__:

- Active learning: Create diagrams when you're learning.
- Introduction of using k8s at a company:
  - Do Discovery sessions: With each team - before & during migration process. See what they need.
  - Get Documentation Feedback - on each part of the k8s guide.

Milestones:

- Learn
- Listen
- Level Up

## Talk 3

__Topic__: Bridging Dev and Ops with eBPF: Extending Observability Upwards and Downwards

__Takeaways__:

- What Javascript is to the browser, eBPF is to the Linux kernel.
- eBPF-powered networking & security can bring cloud native observability & routing
- Cilium
  - replace IPtables
  - repace sidecar proxy for service mesh
- Hubble
  - fine-grained network observability (from the kernel)
  - exports to SIEM
  - support for OpenTelemetry
- Parca: Contiunous profiling https://www.parca.dev/



## Talk 4

__Topic__: Priorities - the art of saying no

__Takeaways__:

- Time is a __finite__ resource
- Urgency is a __trap__
- Urgent-important matrix / Eisenhower Matrix

|                   | Urgent   | Not urgent |
|-------------------|----------|------------|
| __Important__     | Do       | Plan       |
| __Not important__ | Delegate | Eliminate  |

1. Do: Simply do
2. Plan: Spend 10-20% of time
3. Delegate: Don't do. Find someone else to do it.
4. Eliminate: Simply don't do.

How do we know something is important?

- There is no such thing as absolute importance.
- Question to ask: Does this thing directly contribute to my goal?
  - Yes: Important
  - No: Enabler for my goal?
    - Yes: Important
    - No: Not important

> Without a __goal__, nothing is __important__.

Strategy:

- Follow the __value__
- Find important stakeholder
- Important is what thing brings value to stakeholder

Questions to ask:

- ROI Analysis: Time to value ratio
- Next best alternative considerations
- If I do this, what will I __not__ do?

> Prioritization means saying "no" ... more times than saying "yes".

Prioritization:

- What should I drop or postpone to do this?
- How does this request fit into our goal?
- What should I do __first__?



## Ignite Talks (each 5 minutes)

- 6 years and 15 meetups later - how to organize a (DevOps) meetup
  - TODO
- DevOps, ClickOps, GitOps, CloudOps, AIOps… making sense of the Buzzword-Bingo in 5 min.
  - TODO
- Enabling true DevOps organizations with Value Stream Management
  - TODO
- Full-stack DevOps engineers: a myth?
  - TODO
- Platform Teams and Innersource, how to foster acceptance and generate synergies
  - TODO

## Workshop

__Topic__: Engineering Lead Masterclass

__Takeaways__:

- TODO

## Evening Keynote

__Topic__: DevOps - like Riding a Bike or rather like Playing Golf?

__Takeaways__:

- TODO