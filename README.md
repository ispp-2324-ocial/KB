# Knowledge base

This repository serves as Ocial's main knowledge base. Each of the repositories that
are a component of Ocial's system must contain their own wiki and documentation assets,
but everything that gets out of their own scope must be discussed or placed here.

Some examples of those are business rules or functional decisions, since those usually involve
backend and frontend teams working together.

## RFCs

### What is an RFC?

The "RFC" (request for comments) process is intended to provide a consistent and controlled path for new features to
be incorporated into Ocial during the development *(and after the reach of the project has been defined)*.

Many changes, including bug fixes and documentation improvements can be implemented and reviewed via the normal GitHub's Pull Request workflow
in each of the projects that belong to Ocial.

Some changes though are "substantial", and given they can interfere the milestones of the project, they must be put through a bit of a design process and produce a consensus among the team.

### The RFC lifecycle

An RFC goes through the following stages:

* **Pending**: when the RFC is submitted as a discussion thread (under the RFCs category).
* **Active**: when an RFC is acknowledged and undergoing implementation.
* **Landed**: when an RFC's proposed changes are shipped and finalized.
* **Rejected**: when an RFC is officially rejected or dropped.

### When to follow this process

You need to follow this process if you intend to make "substantial" changes to the feature set defined in the project constitution.

What constitutes a "substantial" change is evolving, but may include the following:

* A new feature that creates new API surface area
* Changing the semantics or behavior of an existing API
* The removal of features that are already shipped as part of the release channel.

Some changes do not require an RFC:

* Additions that strictly improve objective, numerical quality criteria (speedup, better browser support)
* Fixing objectively incorrect behavior
* Rephrasing, reorganizing or refactoring
* Addition or removal of warnings

### Why do you need to do this

To fulfill's Ocial target goals, we need to be serious about the planification and stability,
and thus have to carefully consider the impact of every change we make that may deviate from the project milestones and target audience.

These constraints and tradeoffs may not be immediately obvious. However, the RFC process serves to go through a thought process as a team,
so that we can be on the same page when discussing why or why not these changes should be made.

### Gathering feedback before submitting

It's often helpful to get feedback on the concept before diving into the level of API design and use cases detail required for an RFC.
You may start a discussion [under the General category](https://github.com/ispp-2324-ocial/KB/discussions/categories/general) to brainstorm first
or go directly ahead with the process.

### What the process is

In short, one must first get the RFC merged into the RFC repo as a markdown file. At that point the RFC is 'active' and may be implemented.

1. Work on your proposal in a Markdown file based on the template (0000-template.md) found in this repo.

  * Put care into the details: RFCs that do not present convincing motivation, demonstrate understanding of the impact of the design, or are disingenuous about the drawbacks or alternatives tend to be poorly-received.

2. Open a new thread in Discussions and make sure to set category to "RFC".

  * Build consensus and integrate feedback in the discussion thread. RFCs that have broad support are much more likely to progress.

3. Eventually, the team will decide whether the RFC is a candidate for inclusion.

  * An RFC can be modified based upon feedback from the community. Significant modifications may trigger a new final comment period.

  * An RFC may be rejected after discussion has settled and comments have been made summarizing the rationale for rejection. The RFC's associated pull request will be closed.

  * An RFC may be accepted at the close of its final comment period. When the team agrees, the RFC's associated pull request will be merged,
  at which point the RFC will become 'active'.

If the proposal has been approved for inclusion, you can prepare a Pull Request:

Fork this repo.

Create your proposal as active-rfcs/0000-my-feature.md (where "my-feature" is descriptive. Assign numbers sequentially).

Submit a pull request. Make sure to link to the discussion thread.

**Ocial's RFC process owes inspiration from [Vue](https://github.com/vuejs/rfcs) and [React](https://github.com/reactjs/rfcs) processes'.
