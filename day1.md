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
  - Success Factors: 
    - #1 Values (local meetup, no online meetups, experience reports)
    - #2 Know your Crowd => do a survey
    - #3 Gather Interest. Keep talk duration short. Do survey for interests
    - #4 A diverse organizing team
    - #5 Get the word out. Continuoualy and repeatably announce it.
  - What did not work
    - Organizing apero themselves
    - Locations far away from the city center
  - First steps
    - Contribute a talk first
    - Organize within own organization
- DevOps, ClickOps, GitOps, CloudOps, AIOps… making sense of the Buzzword-Bingo in 5 min.
  - BizDevOps: DevOps already includes Business. BizDevOps just means they are focusing on business or that business is the biggest challenge
  - GitOps and {x}-as-code: Tooling
  - SRE & Platform engineering: Scale DevOps.
- Enabling true DevOps organizations with Value Stream Management
  - hm
- Full-stack DevOps engineers: a myth?
  - What skills and traits to look for
    - Eager to make things work
    - Excited about technical challenges
    - Strong sense of ownership
- Platform Teams and Innersource, how to foster acceptance and generate synergies
  - How to get acceptance for internal platforms (API mgmt, CI/CD, etc)
  - Do's
    - Transparency: Code, Test, Issue management etc open
    - Classic product ownership
    - Decentralized development
    - Rules
    - Managing different stakeholders
  - Don't do:
    - No dedicated resources
    - Low/no quality
    - Closed door policies
    - Do not babysit users
- GitHopes & Terrorforms
  - Decoupled pipelines
  - Decoupled teams
  - Decoupled git repos

## Workshop

__Topic__: Engineering Lead Masterclass

- How to measure lead time? => Little's Law
  - Process lead time (PLT) is equivalent to the work in process (WIP) divided by the exit rate (ER). For example, if you have 20 widgets in process and they exit the line at 2 every minute, then you have a process lead time of 10 minutes.

Ladder examples:

Example 1:

- Work hard
- Hire hard working people
- Remove impediments
- Empower teams to see/priorize/remove its own impediements

Example 2:

- Write code!
- Control quality (PR, pairing)
- Build a culture of technical excellence
- Hire someone bettere than yourself to do it

### Apply second order thinking

- First order: I'll fix this problem. Solution oriented, fast and easy.
- Second order: And then what? More deliberate.
- System Impact: How will this affect the system of work?

### Mentors Toolbox

1. Encourage
  - Help people fight self-doubt.
  - You can do it!
  - Thank them (ask if they're okay with public praise). Be sure to make it: "Thank you $name for $explicitReason"
  - Support initiative!
2. Challenge
  - Delegate technical work and non-technical work.
  - Delegate tasks that maximise learning (trade off with speed)
  - Delegate the most interesting work.
3. Coaching
  - Don't solve their problems, ask questions.
  - We'll do an exercise on this in a bit.
4. Share
  - Knowledge
  - Energy
  - Optimism
5. Set rules
  - Less control, more systems.
  - WIP Limits
  - Build it & run it
  - CI with daily push to trunk
  - Every time a new pair to spread knowledge and team work
6. Do things together
  - Pair on anything! Code, architecture, conflict resolution, etc.

### How to build trust

Trust is the most important thing to build!

- Your knowledge
- Your consistency
- Your authority
- Your confidence
- Your market value
- Your ability to manage anxiety

### Recruiting

__Improve quality of candidates by being visible__

- People should know what you do, what technologies you use or create.
- Spread this by sharing at local meetups (or in the remote world, online ones).
- Attract candidates that have the right attitude which in return will drive away bad candidates in the future (protect your culture!).


Tip: Avoid Dunning Krugers!

__Job ad do's and dont's__

Don't do this:

- Hard requirements like 3+ years of k8s experience
- "Strong understanding", "experts" or "deep knowledge"

Do this

- Describe your environment
- What tech are you currently using or thinking of using?
- What will you actually be doing in this role?
- Unfamiliar with some of the tech? Apply anyway!

#### Retention

> One tip to rule them all: Turn seniors into mentors.

## Evening Keynote

__Topic__: DevOps - like Riding a Bike or rather like Playing Golf?

__Takeaways__:

- TODO