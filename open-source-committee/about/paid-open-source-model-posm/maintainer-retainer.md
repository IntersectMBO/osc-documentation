---
description: >-
  This is a working draft. Nothing here should be treated as final until
  formally approved. Formal OSC approval to follow.
---

# 🤓 Maintainer Retainer

## Executive Summary

Maintainer Retainer Program provides recurring funding to experienced contributors responsible for maintaining critical Cardano open-source repositories, ensuring projects remain secure, regularly updated, and actively developed.

## Definitions

**Core Maintainer**\
Senior project steward with final technical authority over a repo’s direction. Owns strategic decisions, governance/policy work, release sign-off, and security-sensitive changes; mentors others and ensures long-term project health.

**Community Maintainer**\
A Trusted-Committer–level maintainer funded via the Maintainer Retainer program to expand capacity around a project. Focuses on day-to-day maintenance and community operations that increase quality and throughput—without holding ultimate decision rights or high-risk credentials. Must meet the Contribution Ladder threshold (≥ Trusted Committer) and pass the program’s 30-day evaluation before ongoing funding.\
\
Contribution Ladder reference: [https://committees.docs.intersectmbo.org/intersect-open-source-committee/policies/contribution-ladder-framework](https://committees.docs.intersectmbo.org/intersect-open-source-committee/policies/contribution-ladder-framework)

## How they differ (at a glance)

| Dimension                    | Core Maintainer                                                                                                                                | Community Maintainer                                                                                                                            |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Primary mandate              | Set strategy, make final technical/governance calls, ensure release quality and sustainability.                                                | Execute and scale day-to-day maintenance; triage, review, test, document, and shepherd contributions to keep velocity high.                     |
| Authority & decision rights  | Final say on architecture, roadmap alignment, releases, and policy within project governance.                                                  | Recommend and implement; proposes changes and participates in reviews, but defers final calls to Core Maintainers/PMC.                          |
| Access level                 | May hold elevated repo permissions and release responsibilities; at least one Maintainer should be an approved “Insider” for security matters. | Standard write/maintain permissions; no admin/secrets or signing keys by default; can be added as “Insider” only if vetted per security policy. |
| Security-sensitive work      | Leads/co-leads on embargoed fixes and coordinated releases.                                                                                    | Assists under direction (repro, tests, docs, backports); escalates promptly; Insider status if/when approved.                                   |
| Release responsibilities     | Owns release criteria and final sign-off.                                                                                                      | Preps changelogs, verifies checks, tags low-risk backports as delegated.                                                                        |
| Program eligibility & review | Typically already at top of ladder; subject to governance expectations.                                                                        | Must be ≥ Trusted Committer and complete 30-day trial; then quarterly/annual performance reviews for continued funding.                         |

## How Community Maintainers assist Core Maintainers

* **Triage & backlog hygiene (as permitted):** label/route issues, reproduce bugs, close stale items, maintain the project board.
* **Code quality pipeline (as permitted):** review routine PRs, enforce contribution standards, add tests, handle dependency and CI updates.
* **Docs & comms (as permitted):** keep READMEs/guides current, draft release notes, respond to contributor queries, mentor newcomers.
* **Security support (as permitted):** assist responders with reproductions, testing, and backports under Insider controls when approved.

### Governance & compliance responsibilities (Community Maintainers)

* **Institute project governance:** help operationalize the project’s agreed governance model (roles, decision processes, voting/consensus rules), and keep MAINTAINERS.md / CODEOWNERS current.
* **OSC policy compliance:** ensure the repository meets Intersect’s Open Source Committee (OSC) policy requirements (licensing, SECURITY.md, CONTRIBUTING.md, release and change-control procedures, code of conduct, DCO/CLA as applicable).
* **Checklists and attestations:** maintain and regularly update compliance checklists; prepare evidence for periodic OSC reviews and audits; flag gaps and propose remediations.
* **Process stewardship:** facilitate issue/PR templates, labeling policies, and RFC/CIP-style proposal flows where applicable; coordinate governance ceremonies (e.g., release readiness, roadmap checkpoints).
* **Risk and quality gates:** verify that pre-merge and pre-release gates (tests, SBOMs, vulnerability scans, dependency policies) are applied and documented; escalate exceptions to Core Maintainers for final determination.

> Program note: Maintainer Retainer requires at least Trusted Committer level and includes a 30-day evaluation plus recurring performance reviews—this is the default gate for Community Maintainers entering the role.

### Eligibility Criteria

To qualify, maintainers must:

* Be active contributors to eligible Cardano open-source repositories.
* Have achieved at least Trusted Committer Level according to the Contribution Ladder Framework.
* Consistently contribute in areas like code commits, issue resolution, documentation, or governance.
* Maintain projects in one of the Incubation, Growth, or Maturity stages per the Project Lifecycle Framework.
* Pass an initial 30-day evaluation period, demonstrating technical capability, responsiveness, and community engagement.
* Commit to following best practices, including open-source governance standards, repository security, documentation accuracy, and community mentoring.

### Project Qualification Criteria

For a project to qualify:

* It must be categorized at the Incubation, Growth, or Maturity stage.
* It must provide critical infrastructure, foundational technology, or developer tooling for the Cardano ecosystem.
* Demonstrate active and significant usage within the Cardano community (developers, dApps).
* Maintain clear governance procedures, an active roadmap, structured issue resolution processes, and up-to-date documentation.
* Obtain formal approval from both the Technical Steering Committee (TSC) and the Open Source Committee (OSC).\


### Funding Structure & Resource Allocation

The Maintainer Retainer Program provides recurring, ongoing financial support to approved maintainers. Funding allocation is executed through the following process:

1. Project Approval:\
   Reviewed and approved by TSC & OSC based on eligibility and project criteria.
2. Maintainer Selection:\
   Maintainers must meet Contribution Ladder requirements and successfully complete an initial 30-day evaluation.
3. Funding Disbursement:\
   Funding is provided on a recurring schedule contingent upon successful quarterly and annual performance reviews.
4. Performance-based Renewals:\
   Continuation of funding depends on maintainers consistently meeting established benchmarks and evaluation criteria.

#### Oversight & Governance:

* Technical Steering Committee (TSC) ensures funding aligns with Cardano’s core infrastructure and technical priorities.
* Open Source Committee (OSC) oversees adherence to open-source best practices, licensing, and security compliance.

### Review & Evaluation Process

The Maintainer Retainer evaluation process is structured as follows:

* Initial 30-Day Evaluation Period:
  * New maintainers must demonstrate contributions, community engagement, and adherence to governance and best practices. A self-assessment report is required at the end of this period.
* Quarterly Performance Reviews:\
  Evaluations every three months include:
* Contributions (commits, PR reviews)
* Security and stability practices
* Community engagement and mentorship
* Documentation quality
  * Consecutive failures result in warnings and potential funding suspension.
* Annual Renewal Review:
  * A comprehensive annual assessment of the maintainer’s effectiveness, continued relevance, and potential succession planning. Results dictate continued funding or reassignment/removal from the program.

### Performance Metrics & Responsibilities

Maintainers must meet strict performance benchmarks, including:

* Regular Code Contributions:\
  Active updates, enhancements, bug fixes, and performance improvements.
* Security & Stability Maintenance:\
  Timely application of security patches, dependency updates, and maintaining zero unresolved critical vulnerabilities.
* Community Engagement:\
  Active support for contributors, responsiveness to community inquiries, mentoring new contributors, and promoting a healthy open-source culture.
* Documentation Quality:\
  Keeping accurate, clear, and accessible documentation (README files, APIs, developer guides).
* Alignment with Roadmap:\
  Activities must clearly support Cardano's long-term technical and infrastructure goals.

### Evaluation Methods Include:

* Commit history reviews
* Issue resolution tracking (via GitHub/GitLab)
* Security audits and dependency checks
* Community interaction logs and feedback
* Documentation reviews

Failure to meet expectations triggers performance warnings, followed potentially by removal from the program.

### Appeals & Reapplication Process

Maintainers facing negative evaluations have structured options:

* Appealing Negative Reviews:
  * Maintainers can appeal within 14 days, providing justifications and evidence of overlooked contributions. Appeals result in either probationary periods or denial of funding.
* Reapplication after Removal:
  * Maintainers removed due to performance may reapply after six months, demonstrating:
* Renewed open-source contributions
* Improved community engagement
* Updated adherence to maintenance best practices
  * Reapplications require endorsement from current maintainers or committee members.

### Governance & Decision-Making

Maintainer Retainer Program governance involves:

* Technical Steering Committee (TSC):
  * Ensures alignment with Cardano's technical roadmap, infrastructure, and security standards. Reviews technical contributions, project approvals, and feature alignment.
* Open Source Committee (OSC):
  * Oversees open-source compliance, community engagement, sustainability, and licensing/security governance.
* Collaborative Decision-Making:
  * Both TSC and OSC must agree on all approvals, reviews, funding renewals, and program terminations. In disputes, joint sessions are held to reach consensus.

\
