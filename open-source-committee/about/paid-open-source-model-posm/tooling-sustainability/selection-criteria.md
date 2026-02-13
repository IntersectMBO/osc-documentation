# Selection Criteria

#### The Tooling Sustainability Program is designed to fund and support critical open-source tools that the Cardano ecosystem depends on. Its purpose is to keep these projects healthy, reliable, and maintainable over the long term by providing structured support and accountability.

#### We focus on projects that:

* #### Improve developer experience (e.g., better workflows, faster onboarding, simplified tooling).
* #### Enhance interoperability between projects and across ecosystems.
* #### Strengthen day-to-day productivity for developers and operators.
* #### Reduce technical debt across the ecosystem by ensuring tools remain modern, tested, and documented.

#### Project Identification and Intake

Projects enter the Tooling Sustainability Program through two pathways:&#x20;

Pathway 1 “Self-Nomination”: A project, individual, or a team submits a tooling sustainability application directly. If the tool is owned, operated, or commercially controlled by a company, the company must be the formal applicant. Additionally, the Open Source Office may refer projects to apply for Tooling support, also as an extension of Project Support Services offerings.&#x20;

Pathway 2 “Committee-Recommendation”: The Open Source Committee and Technical Steering Committee may independently identify tooling that prevents operational risk, ecosystem dependency risk, or security exposure, and submits non-binding recommendations for consideration.&#x20;

Funding for the Tooling Sustainability Program remains open year round, so long as funds are available, for the current funding cycle. Applications are accepted continuously and grouped into review batches for structured review by Committee(s).

#### Evaluation and Qualification - “How the Process Works”

#### Phase 1 — Interest & Eligibility&#x20;

* Confirm to meet all required checklist items (use [the self-attestation script](https://github.com/IntersectMBO/Project-Compliance-Attestation)).
* Submit project through the [ClickUp intake form](https://forms.clickup.com/9015279944/f/8cnmga8-37315/O6P6T73ETVLHJY9C6D) (include self-attestation result as PDF).

### Self-Attestation: As part of the application, projects must complete a self-attestation using the Intersect Open Source Office scripts. This ensures consistent baseline checks before moving forward.

Script location:

[IntersectMBO – Self-Attestation Scripts](https://github.com/IntersectMBO/Project-Compliance-Attestation)

#### How to Use the Scripts

* Follow the Readme:[ IntersectMBO/Project-Compliance-Attestation](https://github.com/IntersectMBO/Project-Compliance-Attestation)
* Run the appropriate script against your repository URL or local path. Each script validates critical areas such as:
* Required files ([README.md](http://readme.md/), LICENSE,[ CONTRIBUTING.md](http://contributing.md/),[ ](http://security.md/)[SECURITY.md](http://security.md))
* Governance and maintainer metadata ([MAINTAINERS.md](http://maintainers.md/), roles, roadmap)
* CI/CD presence and test coverage
* Dependency hygiene (lockfiles, SBOM, dependency update tooling)
* Security reporting and disclosure basics
* Save the output (console log or generated report).
* Attach the pdf results to your application form along with links to your evidence (repo files, CI config, SBOM, etc.).

Outcome:

* Pass: Invited to Phase 2.
* Fail: Feedback provided with remediation steps. Applicants may re-apply once fixed.

#### Phase 2 — Evaluation & Demo (with OSC and Tooling WG)

* Qualified projects are invited to enter a structured evaluation led by the Open Source Committee (OSC).
* Components include:
* Concise project demo (\~5–10 minutes).
* Review of repository artifacts, cross-checked with your attestation output.
* Q\&A session covering scope, technical readiness, governance, roadmap, and security posture.

What reviewers look for:

* Clear problem definition and user need.
* Evidence of adoption or demand.
* Defined path to PoC/MVP with acceptance criteria.
* Demonstrated ability to deliver on milestones.

#### Phase 3 — Selection & Funding Terms

Projects approved by OSC move to funding alignment, which formalizes:

* Milestones (broken into 2–4 measurable deliverables).
* Acceptance criteria for each milestone.
* Reporting cadence (e.g., monthly blog posts, check-ins, milestone demos).
* Disbursement schedule, tied directly to milestone completion.
* Non-funding support (optional): security reviews, governance consulting, documentation support, community testing, analytics setup.

Outcome:

Projects become formally supported under the Tooling Sustainability Program, with sustained backing for successful delivery and long-term maintainability.

Post-Demo Review and Recommendation:\
Following the applicant demo, Open Source Committee (OSC) members will conduct an internal review of the application. This review assesses technical readiness, sustainability alignment, milestone clarity, and ecosystem impact based on the information presented during the demo and submitted materials.

Upon completion of the OSC internal review, a consolidated recommendation, including relevant findings and supporting documentation, is forwarded to the Technical Steering Committee (TSC) for optional technical review and advisory input.

Milestone Definition and Scope Control

For applications that pass technical and program evaluation, a milestone plan is submitted by the applicant/project. Each milestone must define a specific what, why, how, and by when the requested tooling development support will be complete.

Scope is explicitly locked to sustainability objectives. Any work that drifts into net new product development, commercial features, or unrelated research is excluded from this funding path and must be redirected to alternative funding programs.

Final Approval and Async Voting

Once evaluation is complete and milestones are finalized, the Open Source Committee will conduct a vote. A successful vote authorizes funding, the milestone contract is then vetted by Intersect Procurement, and projects are onboarded into the Tooling Sustainability Program.

### Payment Bands (Guidance Framework)

Note: The following bands serve as guidance only. Final award amounts are determined at the discretion of the Open Source Committee (OSC) based on submission quality, impact, and ecosystem priority. Band categories may also change at any time, but notice will be provided. The maximum ceiling for any individual (per project) award is $50,000 USD.

In order to preserve Treasury spend and support up to 20 Tooling projects, The OSC wishes to provide funding in ADA, commensurate with the USD banding approved by OSC.&#x20;

| Band                                     | Work Type                                          | Milestone Payout (USD)            | Criticality Level                         |
| ---------------------------------------- | -------------------------------------------------- | --------------------------------- | ----------------------------------------- |
| Band 0 — Exceptional (Ceiling Tier)      | Groundbreaking or ecosystem-critical tooling       | $35,000- $50,000 (OSC discretion) | Mission-critical or ecosystem-wide impact |
| Band 1 — Core Critical Tools             | Infrastructure, build systems, or protocol tooling | $15,000 – $35,000                 | Essential for Cardano’s operation         |
| Band 2 — High Impact Developer Tooling   | SDKs, testing suites, language tools               | $5,000 – $15,000                  | Widely used by developers but non-core    |
| Band 3 — Ecosystem Utilities & Libraries | Middleware, dashboards, CLI tools                  | $2,000 – $5,000                   | Improves productivity or observability    |
| Band 4 — Experimental / Incubation Tools | New or early-stage repos                           | $500 – $2,000                     | Innovative but unproven                   |

#### Disbursement and Financial Execution

Each payment is contingent upon the successful delivery and verification of the approved milestone. Disbursement may cover maintenance labor for approved sustainability work, security remediation, infrastructure required for tool operation, and documentation or handover outputs.

Milestone payments will be set in ADA commensurate with USD value at the time a Milestone/task is posted.

Participation in the Tooling Sustainability Program does not establish permanent ownership status, exclusive vendor relationships, or automatic renewal rights.

#### Milestone Verification and Oversight

Milestone completion is verified through defined deliverables such as production releases, patch confirmations, documentation publication, audit remediation evidence, or operational stability improvements. Verification is conducted by the Open Source Office with reporting to the Open Source Committee.

Non performance, scope deviation, or failure to deliver may result in milestone rejection, funding hold, scope correction, or non renewal of the project.

#### Program Exit

Funded tooling is subject to periodic review based on milestone performance, ecosystem dependency, and evolving risk posture. Tools may exit the program through successful stabilization and lowered risk profile, replacement by superior tooling, or failure to meet sustainability obligations.\
\
<br>

\
\
<br>
