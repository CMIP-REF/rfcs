# CMIP-REF RFCs

The "RFC" (request for comments) process is intended to provide a consistent
and controlled path for large technical decisions for the REF.

Many changes, including bug fixes and documentation improvements can be
implemented and reviewed via the normal GitHub pull request workflow.

Some changes though are "substantial", and we ask that these be put through a
bit of a design process to ensure that we building what the community needs.

## Table of Contents
[Table of Contents]: #table-of-contents

  - [Table of Contents]
  - [What the process is]
  - [The RFC life-cycle]
  - [Reviewing RFCs]
  - [Help this is all too informal!]
  - [License]
  - [Contributions]


## What the process is
[What the process is]: #what-the-process-is

In short, to get a major feature added to the REF, one must first get the RFC
merged into the RFC repository as a markdown file. At that point the RFC is
"active" and may be implemented with the goal of eventual inclusion into the REF.

  - Fork the RFC repo [RFC repository]
  - Copy `0000-template.md` to `text/0000-my-feature.md` (where "my-feature" is
    descriptive). Don't assign an RFC number yet; This is going to be the PR
    number and we'll rename the file accordingly if the RFC is accepted.
  - Fill in the RFC.
  - Submit a pull request. As a pull request the RFC will receive design
    feedback from the larger community, and the author should be prepared to
    revise it in response.
  - Now that your RFC has an open pull request, use the issue number of the PR
    to rename the file: update your `0000-` prefix to that number. Also
    update the "RFC PR" link at the top of the file.
  - Build consensus and integrate feedback. RFCs that have broad support are
    much more likely to make progress than those that don't receive any
    comments. Feel free to reach out to the RFC assignee in particular to get
    help identifying stakeholders and obstacles.
  - At some point, 

## The RFC life-cycle
[The RFC life-cycle]: #the-rfc-life-cycle

Once an RFC becomes "active" then authors may implement it and submit the
feature as a pull request to the REF repository.
Being "active" is not a rubber stamp, and in particular still does not mean
the feature will ultimately be merged; 
it does mean that in principle all the major stakeholders have agreed
to the feature and are amenable to merging it.

Furthermore, the fact that a given RFC has been accepted and is "active"
implies nothing about what priority is assigned to its implementation, nor does
it imply anything about whether a developer has been assigned the task of
implementing the feature. While it is not *necessary* that the author of the
RFC also write the implementation, it is by far the most effective way to see
an RFC through to completion: authors should not expect that other project
developers will take on responsibility for implementing their accepted feature.

Modifications to "active" RFCs can be done in follow-up pull requests. We
strive to write each RFC in a manner that it will reflect the final design of
the feature; but the nature of the process means that we cannot expect every
merged RFC to actually reflect what the end result will be at the time of the
next major release.

In general, once accepted, RFCs should not be substantially changed. Only very
minor changes should be submitted as amendments. More substantial changes
should be new RFCs, with a note added to the original RFC.


## Reviewing RFCs
[Reviewing RFCs]: #reviewing-rfcs

While the RFC pull request is up, the development-team may schedule meetings with the
author and/or relevant stakeholders to discuss the issues in greater detail,
and in some cases the topic may be discussed at a development-team meeting. In either
case a summary from the meeting will be posted back to the RFC pull request.

A development-team makes final decisions about RFCs after the benefits and drawbacks
are well understood. These decisions can be made at any time, but the development-team
will regularly issue decisions. When a decision is made, the RFC pull request
will either be merged or closed. In either case, if the reasoning is not clear
from the discussion in thread, the development-team will add a comment describing the
rationale for the decision.


## Implementing an RFC
[Implementing an RFC]: #implementing-an-rfc

Some accepted RFCs represent vital features that need to be implemented right
away. Other accepted RFCs can represent features that can wait until some
arbitrary developer feels like doing the work. Every accepted RFC has an
associated issue tracking its implementation in the REF repository; thus that
associated issue can be assigned a priority via the triage process that the
team uses for all issues in the REF repository.

The author of an RFC is not obligated to implement it. Of course, the RFC
author (like any other developer) is welcome to post an implementation for
review after the RFC has been accepted.

If you are interested in working on the implementation for an "active" RFC, but
cannot determine if someone else is already working on it, feel free to ask
(e.g. by leaving a comment on the associated issue).


### Help this is all too informal!
[Help this is all too informal!]: #help-this-is-all-too-informal

The process is intended to be as lightweight as reasonable for the present
circumstances. As usual, we are trying to let the process be driven by
consensus and community norms, not impose more structure than necessary.


## License
[License]: #license

This repository is currently in the process of being licensed under either of:

* Apache License, Version 2.0, ([LICENSE](LICENSE) or https://www.apache.org/licenses/LICENSE-2.0)


## Inspirations

This RFC process is inspired by the [Rust RFC process]
albeit somewhat trimmed down.


