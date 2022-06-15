# Decision Recording Pull Request Validation Protocol

| Status      | proposed                                            |
| :---------- | :-------------------------------------------------- |
| **PR #**    | [31](https://github.com/blindnet-io/openness-framework/pull/31) |
| **Author** | milstan (milstan@blindnet.io)                        |

## Context and Problem Statement

As blindnet [decided](https://github.com/blindnet-io/devrel-management/issues/32) to fully embrace Openness principles, and has put in place a [Decision Framework](https://github.com/blindnet-io/openness-framework/tree/main/DecisionFramework), the need has emerged to establish more clarity in the process of proposing and approving Decision Records.

## Terminology

- The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119 of the IETF](https://datatracker.ietf.org/doc/html/rfc2119)
- We use the terms **decision** and **choice** as defined in the [Decision Framework](https://github.com/blindnet-io/openness-framework/tree/main/DecisionFramework)
- We use the term **Decision Recording**, to refer to recording of any **decision** regardless of the type of document used to record it (such as : DRs (_Decision Records_), SGs (_SMART Goals_) and RFCs (_Request For Comments_)).
- The terms "Assignee", "Collaborator", "Contributor", "Pull Request" (same as "PR"), and "Review" are to be interpreted as described in the [Github Glossary](https://docs.github.com/en/get-started/quickstart/github-glossary)
- A Reviewer is a Collaborator asked to do a Review of a Pull Request

## Decision Drivers

* High clarity for Collaborators and Contributors about who should do what in order for a **Decision Recording** Pull Request to be validated
* Avoid getting the **Decision Recording** Pull Request validation process in a stale point

## Considered Options

Different options have been considered in the discussion that took place in [issue #14](https://github.com/blindnet-io/openness-framework/issues/14). As a result, the following two protocols are defined.

## Decision Outcome

### Validation protocol for template-based decisions

> This protocol applies when recording **decisions** that follow the Decision Framework and use one of [its specific document templates](https://github.com/blindnet-io/openness-framework/tree/main/DecisionFramework#what-template-will-you-use).

In the beginning there are the **Authors** - one or more Collaborators or Contributors.
One of them, the **Corresponding Author**, writes the **Decision Recording** and is committed to championing it through the process.

Collaborators typically have a `@blindnet.io` e-mail address or are otherwise invited to that role.
If an only if, the **Corresponding Author** is not a Collaborator, they MUST find a Sponsor.
A **Sponsor** is a Collaborator who shepherds the decision record through the validation process and makes sure:
- (during the validation process / PR Review) that the **Corresponding Author** is actually heard, the proposal considered, and the process respected
- (after the decision has been recorded / PR merged) the **decision** is applied, respected and understood (i.e. if someone has a question about this **decision**, they should reach to the **Sponsor**)

The **Sponsor**, and the **Corresponding Author** SHOULD be clearly defined in a markdown header of the **Decision Recording** following the decision framework templates.

A Pull Request needs Reviewers and an Assignee.
The **Corresponding Author** and the **Sponsor** are not eligible for those roles. Anyone else is eligible.

Anyone MAY, and at least one of the {**Corresponding Author**, **Sponsor**} MUST designate one or more eligible Reviewers.
An eligible Reviewer MAY designate themselves.

The **Corresponding Author** OR the **Sponsor** MUST assign the **Decision Recording** Pull Request to an eligible Assignee.
The Assignee MAY also be a Reviewer.

The Assignee looks for consensus before merging the **Decision Recording** Pull Request.
The Assignee SHOULD act to have the proposal converge towards a consensus.
The Assignee is sovereign in interpretation of what a concuss is, unless a `FORMAL OBJECTION` has been raised by a Reviewer (according to [Best Practice for Reviews]([review a PR](https://github.com/blindnet-io/openness-framework/blob/main/docs/HOWTOs/PR-review.md#best-practice-for-reviews))).
In that case, the Assignee MUST consider that there is absence of consensus as long as the Reviewer in question has not indicated `FORMAL OBJECTION LIFTED`.
In clear absence of consensus the Assignee closes the request.
It is the responsibility of the Assignee to act and not let PR remain at a stale point.

An alternative **Decision Recording** MAY always be proposed.

Whenever possible (unless they are not eligible, or for other reasons known to be unavailable), the Assignee SHOULD be:

1. `@noelmace` for everything related to communication, openness framework, DevX and DevRel in general
2. `@filipblnt` for everything related to engineering, by default (adding a member of the engineering team as an additional Reviewer whenever needed)
3. `@milstan` for everything related to our company's "vision" and high-level concepts (i.e. high-level product ownership)
4. `@Vuk-BN` for everything related to global executive strategies and finances

When such an assignment is not possible, then the Assignee SHOULD be the first eligible and available person from the above list, in the order from 1. to 4.

### Validation protocol for non template-based documents

> This protocol applies, unless a particular project-related workflow is specified in the project's readme file, when producing other types of documents that MAY also involve more or less normative **choices** and even certain **decisions** (e.g. user stories, specifications, designs, documentation work, code) but that do not use one of the [Decision Framework's specific document templates](https://github.com/blindnet-io/openness-framework/tree/main/DecisionFramework#what-template-will-you-use)

One of the Authors, the **Corresponding Author**, makes a PR.
They invite Reviewers other than themselves.
Anyone MAY [review a PR](https://github.com/blindnet-io/openness-framework/blob/main/docs/HOWTOs/PR-review.md), therefore designating themselves as a **Reviewer**.

The **Corresponding Author** assigns a person (other than themselves, which MAY also be a Reviewer, in the same order as for template-based decisions).

The Assignee looks for consensus before merging the Pull Request.
The Assignee SHOULD act to have the proposal converge towards a consensus.
The Assignee is sovereign in interpretation of what a concuss is, unless a `FORMAL OBJECTION` has been raised by a Reviewer (according to [Best Practice for Reviews]([review a PR](https://github.com/blindnet-io/openness-framework/blob/main/docs/HOWTOs/PR-review.md#best-practice-for-reviews))).
In that case, the Assignee MUST consider that there is absence of consensus as long as the Reviewer in question has not indicated `FORMAL OBJECTION LIFTED`.
In clear absence of consensus the Assignee closes the request.
It is the responsibility of the Assignee to act and not let PR remain at a stale point.

An alternative document MAY always be proposed.

## References

* The [Decision Framework](https://github.com/blindnet-io/openness-framework/tree/main/DecisionFramework)
