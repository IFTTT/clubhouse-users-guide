# Overview

## Why do we need this guide?

Communication is by far the most important capability that ClubHouse provides. ClubHouse is the most important communication tool that we have at IFTTT. If Slack, Gmail, SMS, VoIP and all other communication methods are not available, our business should be able to keep moving forward with ClubHouse. At least temporarily. 😉

Visibility is another _very_ important capability that ClubHouse provides. Though, it's important to understand that the visibility that ClubHouse provides depends on us using ClubHouse in a consistent way.

In order to aggregate ClubHouse data, the attributes related to the entities in the data must have consistent semantics. This document defines the semantics in a way that makes sense to the IFTTT team and sets some basic rules to ensure data consistency.

## Mapping IFTTT Concepts to ClubHouse

The following diagram maps IFTTT organizational and process concepts to ClubHouse features. This mapping provides a clear conceptual understanding of how we use ClubHouse to get work done at IFTTT.

![](https://lh5.googleusercontent.com/mAPpz-MU16a-WOUqAVsRbcl_O20_jAcmmeZe3p635VsHDTx9BuWBQqD3mGyA3t5sP8ScQdCcete45RmUG0Mn3vJHYZP2pvmvCNEFHT6TemlMI3iTjt8l_8IYAnIHZPyY_4ZlsEtK)

This diagram uses [Crow’s Foot Notation](https://en.wikipedia.org/wiki/Entity%E2%80%93relationship_model#Crow's_foot_notation) to show associations, which tells us:

* Projects represent IFTTT components or services and can be associated with many stories
* Milestones represent Impact Cycles and can be associated with many Epics
* Epics may or may not be associated with a single Milestone
* Epics are related to zero or more stories
* Teams represent squads and can be associated with many Epics, Stories and Iterations
* Teams can be associated with many Iterations
* Iterations must be associated with one and only one team
* Stories must belong to one and only one Project, Epic and Team

Note: The above association rules are how IFTTT uses ClubHouse. In some cases ClubHouse will allow the above rules to be broken.

## Time View

ClubHouse allows us to group and track Stories \(the work we do\) in many different ways. These groupings tend to fall into one of two categories:

* Timebox - A way to group Stories into a fixed chunk of time in which work is planned to be done.
  * Typically begins with a planning session and ends with a retrospective.
  * Typically fixed in size and length to help with visibility and estimation.
* Workbox - A set of related work to be done in order to complete a specific goal, feature-set or initiative.
  * A workbox is not constrained by time; it may last be a few days, a few weeks or forever.
  * A workbox can group work using any number of attributes: team, component, service, etc.

### Timeboxes

We use several different timeboxes at IFTTT to track work in the time domain: Impact Cycles, Epics and Sprints.

![](https://lh4.googleusercontent.com/fcF__Q6NQb4MTH6M5Cls0W9aB77UI1pDps9TqqH3pA0VOZi-839FxhEmSHDPCEC6oQ3W6YDj5j0rMIeAvA1Z3HwNNqwgwiKEHUpgKZOjglPW3zuHWb9HSWnIjP9j-e7epPEnc5wf)

#### Impact Cycle \(Milestone\)

An Impact Cycle is a timebox that aims to consolidate and focus work on large initiatives that have strategy-level outcomes typically measured by quarterly metrics. Impact Cycles typically last 6 weeks.

#### Epic \(Epic\)

We use ClubHouse Epics as both a timebox as well as a workbox. An Epic is a group of related stories \(a workbox\) that has a start and end date \(a timebox\), though the start/end dates could be infinite.

#### Sprint \(Iteration\)

A Sprint is a timebox that is used to plan and execute on very small amounts of well-defined work. Sprints typically last 2 weeks.

