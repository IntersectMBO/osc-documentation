# 📜 Governance Policy

NOTE: Please consult the [glossary](glossary.md) for definitions of terms and acronyms.

## High-level overview

This is the high-level structure that this policy is aiming for:

* Development work is organized around individual projects and groups of projects.
* Projects are autonomous and consensus-driven, but also equipped with an official and transparent decision-making body.
* The Technical Steering Committee is ultimately responsible for ensuring that the principles are followed, and has a formal decision-making body that can progress even when consensus is hard to find.
* Projects are accountable to the TSC, and this should affect their behaviour, but this accountability is only formally invoked in exceptional cases.

## Conformance

This policy mostly aims to provide a sensible default. Therefore most of its statements use "should". There are a few exceptions, and these are indicated by the use of "must".

See the [policy introduction](../introduction.md) for further discussion.

<details>

<summary>Examples</summary>

* The PMC for a meta-project wants to give the person acting as release manager a veto on votes to perform a release.
  * This is perfectly logical and a good way to help ensure the quality of the release.
  * This is assuming that the release manager has merit - if they are simply posted into that role by a company, then it is much less clear that they have sufficient merit to deserve to be able to block a release.
* The PMC for a meta-project wants to form a group of technical experts to do design review for proposals.
  * This is again reasonable and a good way to make it easier for contributors to make substantial changes and be confident that their proposals will be accepted.
  * Again, the members of the group should be meritorious, and the selection process should reflect that.
* The PMC for a project wants to require reviews from specific experts on changes to certain parts of the codebase, using CODEOWNERS or otherwise.
  * This is good practice, and so long as appropriately meritorious reviewers are being chosen it should work well.
  * This is a particularly sensible policy for large projects where individuals may prove themselves worthy of being a Committer, but only on certain parts of the codebase. The Committer role is too binary to accommodate this, so it is sensible to add a mechanism like CODEOWNERS on top.
* The PMC wants to give Maintainers veto rights on PRs.
  * This is fine: if a project wants to have more powerful Maintainers that’s not bad _a priori_.
  * Care should be taken that the Maintainers are not then more powerful than their Merit, and more scrutiny should be applied to giving people the role.
  * If this is part of a move towards increased centralization of authority then it might be bad from a Sustainability perspective.
* The PMC wants to use a communication channel that meets the requirements, but is different from the channel used by most other projects.
  * Having non-standard “interfaces” makes the project harder to work with, and makes it harder for contributors to know how to interact with it, so this is mildly damaging to Sustainability. It may nonetheless be a good decision if there are other reasons to do it.
* The PMC wants to elect a “Benevolent Dictator For Life” (BDFL) and then have them make final decisions without recourse to the TSC.
  * This is problematic: without the TSC as part of the escalation chain we cannot be sure that we maintain the Legitimacy of the project. Having a BDFL is also bad for Merit (in the future other contributors may be more meritorious) and Sustainability (better to have a wider set of competent contributors)

</details>

## Decision-making

Decision making should generally be done in a consensus-seeking manner. That is, ideally decisions should have consensus, but we do not generally formally require that. If consensus fails we have more structured methods available (escalation).

The general decision-making process is (in order):

1. [Lazy consensus](https://community.apache.org/committers/lazyConsensus.html): just act based on what you think people will want. If nobody objects then everything is fine.
2. [Consensus-building](https://community.apache.org/committers/consensusBuilding.html): seek indications of consensus from the relevant group
   1. Voting: the relevant group votes explicitly (this is an example of consensus-building since it aims to get the group to come to a more explicit consensus)
3. Escalation: the issue is raised to a higher decision-making body

<details>

<summary>Rationale</summary>

Consensus-seeking decision-making lets us use the consensus-based methods that are common in other open-source projects, which tend to operate smoothly and with low overhead the majority of the time. In cases where consensus cannot be found, or where there are fundamental conflicts with the principles, we have an explicit escalation path that allows us to still make decisions.

</details>

<details>

<summary>Examples</summary>

* An established committer makes a PR, and…
  * Merges it themselves
    * For uncontroversial things, using lazy consensus like this is fine. This does require people to use their judgement about what things are likely to be controversial and so need more discussion.
    * Projects may want to add additional guidelines saying that people should not do this, or should require a review before merging. That’s also fine.
  * Gets a review from a fellow committer before merging
    * This is generally a good idea. This is also a small example of consensus-building by seeking input from another contributor on whether the idea is good or not.
  * Brings it to the PMC meeting for discussion before merging
    * This is a good idea if the contributor feels unsure about whether the change is going to be agreeable or not. Discussion might also happen on other communications channels.

</details>

### Voting

Voting is a simple way to build consensus, by asking each member of the group to explicitly state their preference. Voting can be used either to seek a binding consensus, or simply to get a partial gauge of sentiment.

The standard voting process is for voters to issue one of the following votes:

* +1: positive vote
* 0: abstention
* -1: negative vote

Normally when seeking a binding decision, a majority should be sufficient to decide in favour of a motion, but in some circumstances it may be appropriate to treat any negative vote as a veto. This is because the point is to elicit a group consensus: if the vote does not seem like enough for the group to settle on the outcome, then it may be necessary to escalate.

<details>

<summary>Rationale</summary>

Voting is a standard and easy way of building consensus. It is also flexible: it can be used to make a hard decision, or just used as way of gauging consensus.

</details>

<details>

<summary>Examples</summary>

* A project wants to adopt an auto-formatter. Much discussion is had and there is no consensus, but nobody is going to be that put out by not getting their favourite outcome, so the PMC just votes and takes the majority option.
* The PMC votes on whether to accept a controversial patch. There is a majority, but several of the most knowledgeable committers vote against, citing security concerns. The PMC does not feel like they have consensus despite the majority and decides to escalate.
* A controversial change is proposed that would change the future trajectory of the project, but not in a way that the TSC will care about. The PMC decides to agree on a formal voting threshold for deciding and hold a binding vote.
* A committer wants to make a minor change. Nobody has very strong opinions, and so the secretary puts it to a vote. A few "+1"s come in, and nobody votes against, so the committer continues on the basis of some positive sentiment.

</details>

### Escalating issues

Issues that a group cannot resolve themselves must be escalated so that we can continue to make progress. These can be technical problems, social problems, or conflicts between principles.

The default escalation pathway is:

1. The Project Management Committee
2. The meta-project Project Management Committee, if there is one
3. The Technical Steering Committee

Anyone can escalate an issue. Issues raised by Committers _must_ be considered by the relevant body, other issues should be considered.

<details>

<summary>Rationale</summary>

In order to maintain Legitimacy, projects _must_ remain accountable to the Technical Steering Committee (TSC). That means that the TSC has to operate as the final decision-making body for disputes. But the TSC cannot arbitrate everything, so we have to have a sensible chain of decision-making bodies between an individual contributor and the TSC.

We restrict the _right_ to be heard to Committers in order to avoid the risk of being flooded with meritless issues. However the intention is that attention should always be paid to meritiorious issues.

</details>

<details>

<summary>Examples</summary>

* Two contributors disagree about whether a patch should be accepted or not.
  * This may just be a simple disagreement that should be escalated to the PMC, but might go further than that depending on how tricky the issue is.
* A contributor makes a significant contribution, which is rejected by the PMC for not being good enough quality. The contributor thinks that this is incorrect, and it is good enough. They appeal to the TSC.
  * This is a more serious problem. They might also want to appeal to the OSC if they think the PMC is actually behaving badly, not just mistakenly.
* There is a proposal to implement a CIP that was accepted and planned for by the TSC. A highly respected contributor believes that there is a problem with the proposal and refuses to accept it.
  * This is a conflict between Legitimacy and Quality
* Security issues are sensitive, and so must not be disclosed publicly
  * This is a conflict between Quality/Sustainability and Transparency
* A well-regarded contributor is a member of the PMC but consistently behaves badly
  * This is a conflict between Merit and Sustainability

</details>

## Projects

A project is the unit of organization of software development at Intersect. A project consists of one or more source code repositories and the people who work on them. Every source code repository in the Intersect organization must be owned by a project.

A project is governed by a committee of its committers, the Project Management Committee (PMC).

A project should have a single "main" repository. Any project-level information should be recorded in the documentation for this repository, and all other project repositories should clearly point to it in their documentation. The following project-level information must be included:

* The project's decision-making process
  * This should include a link to the decision-making section of this document, but should also note any deviations or additions
* The membership of the PMC
  * This can just be a link to the corresponding GitHub team
* The location of the project's public communications channels (see below)

If a project has multiple repositories, then the set of committers must be the same across all of them.

Multiple projects can be grouped into "meta-projects". The PMC for such a meta project is comprised by one elected member of each project and projects may be added/removed to the meta-project with the consent of both PMCs to facilitate cross-project collaboration. The meta-project PMC is then part of the escalation chain and other policies apply just the same.

<details>

<summary>Rationale</summary>

Projects are intended to map closely onto existing normal development activity.

We require a uniform set of committers across the project because we have tied governance to participation: if the set of committers is different, it is less clear who should get a say in what.

Intersect owns some large, complex projects such as Cardano, and so some framework like "meta-projects" for cross-project coordination and decision-making is essential.

</details>

<details>

<summary>Examples</summary>

* Project X has three dependencies Y, Z, and Q. In addition, there is project R which provides tools for deploying X, and some individuals who act as full-time release managers for X. In this instance it would be appropriate to form a meta-project to collect all of this work.

</details>

### Project Management Committee

The PMC is a committee which consists of all the Committers of the project. The PMC is responsible for making project-level decisions and appointing Committers.

The PMC has two non-development roles associated with it, the Chair and the Secretary. The Chair is responsible for organizing and running meetings, and the Secretary for keeping written material in order. The Chair and the Secretary are elected by the PMC. The Chair and the Secretary need not be Committers. If there is no Chair or the PMC is failing to appoint a Chair, then Intersect may appoint an interim Chair.

PMC meetings should be held regularly, be public, and be advertised on the public communications channel and in the project documentation. Committers have a right to speak, others may be allowed to speak at the discretion of the Chair.

The PMC should make decisions in the usual consensus-seeking manner. If it needs to vote, the Committers are the voters. Votes should be held via the public communications channel to ensure that Committers are notified.

### Roles

Roles are per-project. All roles are non-exclusive, an individual may hold any number of roles.

The role assignments for a project should be listed in a discoverable way. For roles associated with membership of a GitHub Team, it is enough to say that the team exists.

#### Development

There are three primary roles associated with doing development work.

1. Contributors are anyone who contributes to the project in any way. There is no formal requirement to be a contributor, nor do they have any formal powers, but it is useful to have a way to refer to them.
2. Committers are people who have been given commit access to the project. Committers are also required to participate in the project governance process - the two go together.
3. Maintainers are individuals who have contributed in a sustained and substantial way to the project, and who commit to keeping the project healthy. Maintainers have additional responsibilities but no additional power (versus Committers). They are likely to be influential, but this is because influential people should be made Maintainers, rather than vice versa.

<details>

<summary>Rationale</summary>

* Maintainers
  * We know there are likely to be paid maintainers, it is helpful to recognize this in some official way.
  * The Maintainer role exists primarily as an honorary one. This gives us a way to recognize the people who are in practice giving lots of time and attention to maintenance (and likely being paid for it).
  * The Maintainer role doesn’t come with additional power. Maintainers will likely have additional influential through their merit and reputation alone.
* Project leads
  * We do not have a concept of a single project lead.
    * In the future we will hopefully have many groups of contributors, all of whose voices should be heard. This is somewhat incompatible with having a single nominated project lead.
    * We could have elected project leads. However, this adds a possibly-unnecessary additional power structure, and we have to define what their powers are.
  * This does not mean that there may not be more traditional team structures associated with the project contributors.
    * For example, a company may have a team working on `cardano-ledger` and that team will probably have a team lead and be organized in typical company fashion. But the company-appointed `cardano-ledger` team lead does not have any special status when it comes to making decisions for the `cardano-ledger` Intersect project.
    * As an example of how this works outside of Intersect, consider GHC. IOG has a GHC team, with an appointed team lead. But the IOG GHC lead doesn’t have any particular sway in the leadership of GHC-the-OSS-project, which is led by its major contributors and its BDFL. In practice, as a good contributor the IOG GH Clead does have some voice, especially in areas where he works a lot, but this is more about his history of contribution than the fact that he is the IOG GHC lead.

</details>

#### Non-development

There are two non-development roles associated with the PMC, Chair and Secretary, which are described in the PMC section.

Individuals may occasionally be given the Administrator role. This is a very powerful role and should only be used for a few highly trusted staff at Intersect who can implement dangerous actions when necessary.

#### Role and Team Summary

| Role          | Rights                                                                                | Responsibilities                                                                                                         |
| ------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Contributor   | Open issues; attend PMC meetings; make code contributions                             |                                                                                                                          |
| Committer     | As Contributor; speak at PMC meetings; member of `<project>-committers`               | Attend PMC meetings; vote on PMC motions                                                                                 |
| Maintainer    | As Committer; member of `<project>-maintainers`; maintainer of `<project>-committers` | As Committer; ensure that pull requests and issues are reviewed in a timely fashion; maintain the health of the codebase |
| Administrator | Member of `<project>-admins`; maintainer of all the `<project>-*` teams               | Should only take action when directed to by the appropriate authority.                                                   |
| Chair         |                                                                                       | Organize PMC meetings; report on the PMC’s activities to Intersect                                                       |
| Secretary     |                                                                                       | Take minutes during PMC meetings; ensure that minutes are published publicly; send out votes and tally responses         |

| GitHub Team             | Permissions                                               | Notes                                                         |
| ----------------------- | --------------------------------------------------------- | ------------------------------------------------------------- |
| `<meta-project>`        | Parent team the projects associated with the meta-project |                                                               |
| `<project>`             | Parent team for teams associated with the project         |                                                               |
| `<project>-committers`  | Write                                                     |                                                               |
| `<project>-maintainers` | Maintain                                                  |                                                               |
| `<project>-admins`      | Admin                                                     | Only appropriately vetted Intersect staff can be in this team |

As usual, projects may augment these as they see appropriate, but they should try to keep any additional teams within the appropriate parent teams.

<details>

<summary>Examples</summary>

* A meta-project wants to have a team of "backup superusers" who can perform privileged actions when the normal maintainers are not available.
* A meta-project wants to have a release management team with additional privileges, to which people are temporarily assigned when they manage releases.
* A project wants to form a documentation team with no additional privileges for use in CODEOWNERS for for `@`-mentioning.

</details>

### Communications

Projects _must_ have a primary public, durable, and asynchronous public channel. Meeting minutes and votes _must_ be sent out on this channel. This _must_ be on a standard Intersect platform (TBD).

Projects _must_ also have a public, real-time chat channel for discussions. This _must_ be on a standard Intersect platform (TBD).

<details>

<summary>Rationale</summary>

Following the principle of Transparency and to enable voting, projects need to have a communication channel that is accessible and public. In order to ensure that discussion remains available for the long term, it should also be durable (i.e. no message expiry, ideally not reliant on ephemeral hosted or paid services).

It is quite beneficial for all the projects to use the same communications platforms. This minimizes friction between projects, and makes it easier for people to know how to contact them. That is why the choice of platform is specified as a "must".

</details>
