# Day 2

Summarizes day 2 of the DevOpsDays Zurich 2023.


## Keynote-Speaker

__Topic__: Developer Productivity Engineering – The Next Big Thing in Software Development

__Takeaways__:

- [Coding War Games](https://fs.blog/increasing-the-productivity-of-computer-programmers-and-engineers). Goal: Figure out good traits of efficient developers
  - Non-Factors: Programming Language, Years of Experience, Defects, Salary
  - Factors:
    - Paired programmers from the same org performed at roughly the same level
    - Average difference was only 21% between paired programmers
    - They didn't work together on the task.
    - Difference between developers of different organizations was 1:10
  - Conclusion: 
    - Some companies are doing a lot worse than others.
    - It comes down to developer experience at a company.
    - 10x engineering is manufactured, not born.
- DPE - Developer Productivity Engineering - should be a core discipline at every company
- Predictive Test Selection - Use ML to select which tests to run. Only use pre-merge!
  - [White Paper](https://research.facebook.com/publications/predictive-test-selection/)
- Correct question to ask: Is the (feedback) cycle as fast as it can possibly be?
- Idea: Measure local build time and failure rates across organization.

> It is staggering with how much toil, friction and frustrations engineers are willing to put up with.

> The world should foster developer joy.


__Book Recommendations__:

- Peopleware: Productive Projects and Teams
- [Developer Productivity Engineering Handbook](https://gradle.com/developer-productivity-engineering/handbook/)
- Phoenix Project or The Goal

## Talk 1

__Topic__: Great Security is One Question Away

__Takeaways__:

- Sanitize and Validate the Input - check what you get from your user. Remember what is your biggest asset and protect it.
- Hire Robots - it is unfair and unrealistic to expect developers to remember about every edge case. Delegate and automate security using DAST and SAST scanners.
- CIA Triad
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

> The one question to ask: How can the CIA of this project be broken?

- When should we ask this question?
  - => Shift left security. Do it during design phase.
- How to implement CIA Triad?
  - Present it to your peers.
  - Discuss it with your team.
  - Make it part of your process.
  - Add it to doc templates

## Talk 2

__Topic__: Development process of Cloud native applications - a story of transformation

__Takeaways__:

- Confidently: single trunk
- Deliver changes: feature driven developer process changes
- Daily: daily deployment to production

Conclusion:

- => Build a paved road.

__Ideas__:

- Integrate the following into a developer portal:
  - Feature Toggles
  - Environments, Deployments, Configuration

__Tools__:

- [CNCF Landscape](https://landscape.cncf.io/)


## Talk 3

__Topic__: Effective Observability in Microservice Architectures

__Takeaways__:

- Make building observable services easy
- Support engineers in refining their skills
  - Standardize on-call training. Make sure it's clear what it means to be on-call.
- Embed observability into your culture


- Culture change should happen both bottom-up and top-down at the same time.

Best practices:

- Event-driven telemetry
- Standardize instrumentation
- Use auto instrumentation first
- Use manual instrumentation strategically

How to choose a tool?

- What observability gap does it fill?
- How compatible is it with our platform vision?
- How easy is it to use?
- Does it provide our support needs?

## Talk 4

__Topic__: Compliance by design | Continuous Compliance

__Takeaways__:

Lessons:

- Compliance will get more complex.
- Compliance is valuable (beyond getting sued).
- Compliance is optional (to a degree).

Conclusions:

=> Shift left compliance.

Summary:

- Agile compliance is possible
- Think broad
- Ensure shared objectives
- Shift culture and process
- Think DevOps

__Links__:

- https://www.beautifulabstraction.com/compliance-by-design/

## Ignite Talks (each 5 minutes)

- The symbiosis of Continuous Deployment and Stability
  - Quality brings Speed. And Speed brings Quality.
- What Is Great About a Modern Monolithic Application?
  - Positive: One repo, one endpoint, one binary, one command, one deployment, one build command, one CI pipeline, one doc, one version
  - Negative: No feature subset, no "simple" mode. Though: Dev vs Prod mode
- The Neuroscience of Communities
  - Serotonin
- The big 3 in automation: Playwright vs Cypress vs Selenium
  - Selenium: Cool, many browsers through drivers
  - Cypress: Cool, same language as frontends, no drivers, but only one tab.
  - Playwright: Uses Websockets to issue commands to browser (fast), but it's limited as it's new.
- Jumping from Bi-Monthly to Daily Releases: Our Journey
  - Story time.
- From Dev || Sec to Dev && Sec
  - Shift left security
  - Invest in the culture.
  - Invest in the right tools and automation.
- The environmental impact of software
  - CO2 reduction measures in order of impact
  - [Estimator](https://github.com/abeggchr/environmental-impact-estimator)
