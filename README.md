# Notes on [DevOpsDays Zurich](https://www.devopsdays.ch/) 2023

- [Day 1](day1.md)
- [Day 2](day2.md)

## Key Takeaways

- Psychological Safety: This is what helps us feel safe:
  - Failure = ok
  - Have open conversations
  - Be willing to help
  - Embrace diversity, equity & inclusion
- Reliability
  - The goal is not 100% uptime.
  - Incident Management
    - What the heck?! => Incident status
    - What was that? => Postmortem
    - How's it going? => Periodic reviews
  - Real-time incident management
    - Use chat & live document (i.e. Google Docs)
    - External people read the chat & doc, they don't ask questions
    - People can offer help, but the response team first has to ack' for them to start helping
  - Periodic Reviews
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
      - Interrupts: Consider a paging "budget", (e.g. max 2 per on-call shift)
      - Morale: A happy team is a reliable team
    - Look forward:
      - Forecast: work to be done
        - What's in the reliability backlog? What might prevent it from getting prioritized?
      - Plans
        - Are stakeholders expecting improved reliability? Can we achieve it?
        - What launches are coming, for this team or related teams?
        - What known future bottlenecks/deprecations/etc can we prepare for?
        - How does the team's work align to (ongoing or emerging) organizational strategy?
- What Javascript is to the browser, eBPF is to the Linux kernel.
  - eBPF-powered networking & security can bring cloud native observability & routing
- Time Management
  - Eisenhower Matrix:
    1. Important & Urgent         => Do: Simply do
    2. Important & Not Urgent     => Plan: Spend 10-20% of time
    3. Not Important & Urgent     => Delegate: Don't do. Find someone else to do it.
    4. Not Important & Not Urgent => Eliminate: Simply don't do.
  - How do we know something is important?
    - Question to ask: Does this thing directly contribute to my goal?
      - Yes: Important
      - No: Enabler for my goal?
        - Yes: Important
        - No: Not important
    - Without a __goal__, nothing is __important__.
    - Strategy:
      - Follow the __value__
      - Find important stakeholder
      - Important is what thing brings value to stakeholder
    - Questions to ask:
      - ROI Analysis: Time to value ratio
      - Next best alternative considerations
      - If I do this, what will I __not__ do?
    - Prioritization:
      - What should I drop or postpone to do this?
      - How does this request fit into our goal?
      - What should I do __first__?
- Hiring
  - What skills and traits to look for
    - Eager to make things work
    - Excited about technical challenges
    - Strong sense of ownership
  - People should already know what you do, what technologies you use or create.
  - Retention: One tip to rule them all: Turn seniors into mentors.
- Internal platforms (API mgmt, CI/CD, etc)
  - Do's
    - Transparency: Code, Test, Issue management, etc. => open
    - Classic product ownership
    - Decentralized development
    - Rules
    - Managing different stakeholders
  - Don't do:
    - No dedicated resources
    - Low/no quality
    - Closed door policies
    - Do not babysit users
- Engineering Lead
  - Apply second order thinking
  - Mentor's Toolbox:
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
  - How to build trust
    - Trust is the most important thing to build!
      - Your knowledge
      - Your consistency
      - Your authority
      - Your confidence
      - Your market value
      - Your ability to manage anxiety
- Developer Productivity
  - 10x engineers are a myth. The development environment at the company makes the difference.
  - The discipline is called DPE - Developer Productivity Engineering
  - Question to ask: Is the (feedback) cycle as fast as it can possibly be?
  - Build a paved road.
  - How to measure lead time? => Little's Law
  - Quality brings speed. And Speed brings quality.
- Security
  - Shift left!
  - CIA Triad questions during design phase:
    - Confidentiality: We want secrets to be secret.
      - Who can see this resource?
      - How do we store credentials?
      - Do we put sensitive data into logs?
    - Integrity: We get what we expect.
      - Who can create, update, remove a resource?
      - Do we have a way to see a potentially malicious actor who deletes all resources at once?
      - What if someone sends malicious data via form to perform an SQL injection?
    - Availability: We can always access the information.
      - Is this endpoint rate-limited?
      - What happens when an external product we rely on is unavailable?
      - How is a database migration performed? Is there a need for a maintenance window?
      - Is a person on support and on-call informed about this?



### Book Recommendations

- Team Topologies
- Thinking Fast and Slow
- Drive: The Surprising Truth About What Motivates Us
- Peopleware: Productive Projects and Teams
- Developer Productivity Engineering Handbook
- Phoenix Project or The Goal
