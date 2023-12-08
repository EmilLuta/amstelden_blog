---
author: Emil Luta
pubDatetime: 2023-12-07T16:00:00Z
title: Promotion Plan Senior Engineer to Principal Engineer
postSlug: promotion-plan
featured: true
draft: true
tags:
  - promotion
  - principal
ogImage: ""
description:
  A small doc describing Emil's promotion plan from Senior Engineer to Principal Engineer @MatterLabs
---

## Context

Emil recently moved from Web2 to Web3 company. His knowledge in the area is rather shaky. He's been with MatterLabs for 8 months. During his tennure, there are 3 noticeable projects delivered:
- On-call Consolidation -- As part of high availability priority focus for 2023, Emil improved the operational load and outages by reworking how the team operated. He introduced processes (Operational Review) and made changes to the current workflows that reduced the outages from 1 per week to 1 every month and a half. Number of tickets also got reduced by 90% and on-call burden reduced by more than 66%.
- Prover subsystems onboarding -- Emil onboarded the prover subsystem, along with Coleague. As Coleague left the company, Emil will inherit ownership of prover subsystems. In the full product, prover subsystems is the component that will prove transitions from state A to state B. It consists of Witness Generator, Witness Vector Generator, Provers and Proof Compressors. Alongside, there are supporting infrastructure to keep everything running, namely Proof Data Handler, Prover Gateway and Basic Witness Input Producer.
- Release of Boojum -- Boojum is the new, faster version of proof generation. This release has been postponed multiple times and it had no owner actively driving it. Emil rose up to the task, designed a plan, coordinated the relevant parties and executed the release as announced on the plan. There were no date slips, the release is successful.

Emil's got his first set of feedback from various stakeholders, as follows a few highlights from those:

### PE
- PEs own big components. I don't yet see one for you.
- All PEs provide fantastic CRs proactive. I don't see you involved enough.
- PEs work together to deliver initiatives (for instance, code quality). There's been little input from you in this area
- Personal initiative -- It's hard to observe this from you. You'll need to market yourself better here.
- Delivering results -- I need to see more code, there's not enough data points. I need more code submissions
- Wrap up On-call -- you have this ongoing, but I see no closure in sight. If you want to mark it as done, announce it close and move on.

To be inclined, I expect to say the following:
- Emil is very vocal in Slack, educates people, does code reviews and he's proactive with it. I don't have to summon him, he appears where he's relevant. Helps the team become better
- When people come to Emil, he helps them and they're unlocked with their tasks.
- Emil delivered this big piece of work. In here, he had no help and drove the entire work forward by himself.
- Emil is looking around the corners to better improve the team.

### Manager
- I'd like to see more ownership. For instance, the metrics for on-call are not great. We've improved it a bit, but still not perfect. I also had some very targeted questions on how on-call works, and you couldn't answer. You came back with answers, but I expected you to know them.
- On communication with DevOps, yes, we don't own our alerts, but I think you could've pushed further. I'm not 100% satisfied with the result and I think there'll be more work left there.
- Your main priority is technical work. Proactive in PRs, more code delivered.
- Get more involved in architecture discussions.

Next steps for you would be:
- Direct manager has to nominate you. Other folks have to approve (other managers) during the calibration meeting.
- The biggest difference I see compared to other PEs is technical ability. They are all stellar in Rust.

### Skip Manager:
- No improvement data points -- Emil reads that as his work not being visible enough for leadership

The way I see it, there's 3 directions for you to look at, as you move up:
- scope
- impact
- autonomy

Today there's a big gap on prover subsystems, I want to hear more of what are your plans there.
Cryptography team doesn't operate as a software engineering team. As time goes by, I want us to encroach more and more on their domain.
Strategically, we have a gap and it is an impactful place to be. We want parts of the system where Manager is not needed

## Problems

Distilled from the above feedback, those are the opportunity areas identified for Emil:

1. No promotion project
2. Low amount of code submissions
3. Poor visibility on architecture decisions (Pull Requests, Slack Threads, Documents)
4. Poor visibility on leadership

## Plan

**TL;DR**
- Decouple server from prover project
- Productionize Boojum project
- Proving speed up project
- Up-to-speed code architecture project
- Rust + Ethereum ramp up
- 1o1s

This underlines how each data point will be tackled:

For point 1, Emil will own Prover Subsystems. There are 3 areas of improvement:
- Decouple the server from prover subsystems
- Productionize new boojum implementation
- Improve proving performance (reduce time from witness generation data hitting the database to proof being sent to server)
Given a strong execution this should be enough. Extra points for addressing the ongoing PE initative (code quality improvements -- prover is a known bad code area) and having more code submissions.
Note: All 3 projects are tracked by leadership. Flawless planning and communication of execution are extra points.

For point 3, Emil will introduce a process in his routine. Every day, he will shift through all open PRs, circle all Slack Threads (saving for later those that have not been finalized to cycle through next day) and weekly look through the documents database.

For point 2, Emil will get more visibility from his plan on point 1 and 3. Additionally, Emil will brush up on his rust knowledge (there are 3 personal projects that need to be done) and get up to speed with the code base. Additionally, Emil needs to plug himself into the Ethereum ecosystem. For this, Emil will go through the whitepaper and the entire website. Emil will map MatterLabs infrastructure to existing L2s and to Ethereum itself.

Point 4 is addressed by point 1s note. Additionally, Emil sets up more 1o1s with his Skip Manager.
Note: Boojum release is a huge step towards visibility.

## Timeline


**TL;DR**
- Decouple server from prover project
- Productionize Boojum project
- Proving speed up project
- 1o1s


Next promotion cycle is ~end of April.

2024

Every week, Emil needs to:
- Check Slack Process
- Check PR Process
Every month, Emil needs to:
- Check Document Reading Process

Week 18
- Buffer

Week 17
- Prover speed up milestone 1 completed & announced

Week 16
- 1o1 with my Skip Manager
- 1o1 with PE

Week 15
- Announce productionizing effort done (plenty of time left-over in case dates slip)
- Deal with any left-overs

Week 14
- Integration tests for prover subsystems

Week 13
- Productionize Prover Compressor

Week 12
- Productionize Prover

Week 11
- Productionize Witness Vector Generator

Week 10
- Productionize Witness Generator

Week 9
- 1o1 Skip Manager
- Productionize Prover Gateway

Week 8
- Productionize Prover Data Handler

Week 7
- Decouple server from prover project is done (2 weeks before schedule, plenty of slack if things go south)
- 1 day off
- Ethereum whitepaper end

Week 6
- Productionize BWIP (new alerts, new monitoring, new dashboard, new runbooks, CI tests, documentation) and announce productionizing initiative (doc might be needed)
- 1 day off
- Ethereum whitepaper start

Week 5
- Rewire the Prover oncall
- Learn how the monitoring stack works
- Ethereum website end

Week 4
- Split leftovers
- Discuss plan on speeding up prover with leadership (plan is to get more resources to help in this area; this will be split in multiple milestones, we'll aim for first milestone, which is to be discussed, agreed & funded)

Week 3
- Create doc for what's left for decoupling
- Create doc for productionizing the existing stack
- Create doc for speeding up proving
- 2 days off

Week 2
- Deploy & Monitor BWIP
- 1 day off
- Finish rust project 3

Week 1
- Finish PRs for BWIP
- Offboard server oncall, onboard prover oncall
- Ethereum website start

2023

Week 52
- Remove old prover from the system
- Start work on rust project 3
- both rust projects 1 and 2 are done
