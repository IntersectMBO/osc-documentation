---
description: >-
  This is a comprehensive assessment by the Open Source Office to analyze the
  maturity level, with the assistance of AI, of all projects currently under
  Intersect.
---

# 🥸 Project Maturity Tiers (2025)

### _Note: This process is currently underway where the OSO is working with the individual projects teams to validate results, so some project ratings are subject to change. Only 66 repos have been analyzed with more to follow._

### Executive Summary

This evaluation reviews the maturity of 66 public repositories maintained under our organization. Each repository was assessed across three critical domains: Documentation, Technical Infrastructure, and Health & Sustainability. Evaluations were derived from both internal metrics and live GitHub data, ensuring an objective and up-to-date analysis.

#### 🔍 Key Findings:

* 48.5% of repositories are classified as Mature, representing stable, governed, and actively used codebases.
* 19.7% are in the Growth phase, showing strong potential but requiring investment in governance and contributor onboarding.
* 21.2% are in Maintenance, continuing to serve important roles with limited active development.
* 10.6% remain in Incubation, needing structure, documentation, and clearer project goals.

#### 🎯 Evaluation Process:

Each project was scored on:

* Documentation completeness (README, governance, templates)
* Technical soundness (CI/CD, testing, linting, security)
* Project health (GitHub metrics: stars, forks, contributors, governance presence)

Final maturity ratings aligned closely with official designations from the governance team. Where discrepancies existed, manual review accounted for internal priorities or strategic value not visible in public metrics.

#### ✅ Outcome:

This assessment provides a clear view of our open source project landscape. It identifies areas for targeted investment, highlights projects ready for promotion, and flags those requiring consolidation or archival. These insights form the basis for prioritizing resourcing and community engagement in our open source strategy.

### Introduction and Purpose

With Cardano’s source code made available as open-source software, Intersects Open Source Office holds an important responsibility to ensure that proper governance is in place alongside healthy development processes.  As the engineering teams we support, contribute to and maintain a growing portfolio of public repositories, it becomes increasingly important to ensure these projects are actively governed, aligned with organizational goals, and supported appropriately based on their lifecycle stage.

This report delivers a structured, cross-functional evaluation of all 66 public repositories under our GitHub presence. The evaluation was commissioned by the Open Source Committee to answer key questions:

* Which projects are stable and production-ready?
* Which are still emerging and need investment in maturity?
* Which are entering a phase of decline, deprecation, or archival?

The assessment aims to provide transparency into the current state of each repository and offer a decision-making framework that supports sustainability, efficiency, and strategic alignment across the open source portfolio. By combining automated technical analysis, documentation audits, and live GitHub metrics with internal knowledge of each project’s intent and ecosystem role, this evaluation gives a comprehensive view of our open source landscape.

Beyond reporting, this work is intended to initiate a sustainable rhythm of lifecycle review and project planning. It helps stakeholders across product, engineering, security, and community functions to identify:

* Projects that deserve investment and visibility,
* Initiatives that require corrective action or clearer ownership
* Legacy components that may be candidates for sunsetting or archival.

Ultimately, the purpose of this assessment is to bring structure, fairness, and forward-thinking strategy to the way we manage our public codebases—ensuring our open source efforts remain high-quality, discoverable, secure, and valuable to both internal teams and the broader ecosystem.

### 2. Evaluation Methodology

The evaluation of each repository was conducted using a multi-dimensional framework designed to reflect the operational health, sustainability, and readiness of open source projects. The methodology integrates both quantitative indicators (e.g., commit activity, file presence) and qualitative signals (e.g., governance maturity, ecosystem role), while incorporating official designations from internal stakeholders.

Repositories were scored independently across three primary dimensions:

#### 2.1 Documentation Maturity (0–9 Points)

The presence and completeness of essential open source documentation was assessed for each repository. These criteria were derived from widely accepted best practices and community standards.

Evaluation Criteria:

* README.md: Overview of the project’s purpose, installation, and usage.\

* LICENSE: Indicates the terms of reuse and distribution.\

* CONTRIBUTING.md: Guidelines for contributing code or reporting issues.\

* SECURITY.md: Describes security contact processes and disclosure policies.\

* CODE\_OF\_CONDUCT.md: Defines behavioral expectations for contributors.\

* Issue and Pull Request Templates: Promotes consistency in contributions and maintenance.\

* Setup & Configuration Instructions: Enables reproducibility and usability.

Each file or component present earned one point for mandatory files, and 0.5 points for having recommended files, contributing to a maximum score of 7. Projects missing several of these components typically reflect lower accessibility and onboarding friction, which impacts community growth.

#### 2.2 Technical Infrastructure Maturity (0–18 Points)

This dimension evaluates the engineering robustness of each repository based on practical software development and DevSecOps practices. The criteria are derived from the internal Technical Assessment Criteria used by engineering teams and adapted for consistency across all public repositories.

Each project was scored across multiple sub-areas of infrastructure maturity, with a total possible score of 18 points. Scores reflect the presence, depth, and automation of technical practices, which collectively determine how scalable and maintainable a project is over time.

| Automated Tests         | Unit, integration, and regression test coverage; enforcement in CI         | 3 |
| ----------------------- | -------------------------------------------------------------------------- | - |
| CI/CD Pipelines         | Presence of pipelines; test/build/release automation                       | 3 |
| Security Scanning       | Use of tools for vulnerability detection (e.g., Dependabot, Trivy)         | 2 |
| Dependency Updates      | Automatic or regular update workflows; package hygiene                     | 2 |
| Linting/Formatting      | Code style enforcement; static code analysis                               | 2 |
| Release Management      | Use of version tags, changelogs, and GitHub Releases                       | 2 |
| Build & Packaging Tools | Automation of builds (Makefile, Dockerfile, etc.)                          | 2 |
| Infrastructure as Code  | Project includes IaC files or deploy artifacts if relevant                 | 1 |
| Platform Integration    | Integration with GitHub Actions, third-party CI platforms (e.g., CircleCI) | 1 |

**Scoring Approach**

* Each repository was manually or programmatically inspected for indicators across these categories.
* Projects with partial implementations (e.g., CI enabled but tests skipped) received proportional scores.
* Repositories with visible release tags, security alert configurations, and automated workflows earned higher scores.

This methodology ensures that technical maturity is not only about the presence of tooling but its operational effectiveness and completeness.

#### 2.3 Health & Sustainability (0–12 Points)

The health of a repository reflects its long-term viability, activity level, and readiness to sustain community contributions or internal dependency. This portion of the analysis was powered by live GitHub data, collected at the time of evaluation.

Scored Dimensions (0–2 points each):

1. Community Engagement – Stars, forks, issue/PR traffic, and evidence of external interest.\

2. Governance & Leadership – Presence of CODEOWNERS, contribution policies, or governance files.\

3. Succession Planning – Number and diversity of active maintainers; reliance on a single contributor.\

4. Ecosystem Importance – Whether the project serves as a dependency or critical integration point.\

5. Activity Trend – Recency and consistency of commits, PRs, and releases.\

6. Sustainability & Risks – Visibility into long-term support, organizational sponsorship, and deprecation risk.

Scores were totaled and mapped into qualitative labels:

* Healthy (10–12): Active, sustainable, and structurally sound.
* Moderate (6–9): Viable but with limitations or improvement opportunities
* Unhealthy (0–5): At risk due to stagnation, governance gaps, or declining interest.

This data-driven approach ensured fairness and comparability across projects of different sizes and scopes.

### Data Integration and Cross-Referencing

To synthesize the evaluation, each repository’s scores across the three categories were aggregated and tallied in the official maturity phase designation listed in the internal governance sheet (Tab 1, Column C). The total scored reflect as follows:

| Scoring Range                                                                 | Maturity Assigned |
| ----------------------------------------------------------------------------- | ----------------- |
| 1-10                                                                          | Incubation        |
| 10-24                                                                         | Growth            |
| 24-37                                                                         | Mature            |
| Was determined by internal review and project purpose                         | Maintenance       |
| Not determined this round given first year unless project is already archived | Decline / Archive |

### 3. Results Summary

Following a comprehensive evaluation of 66 public repositories, each project was assigned a maturity phase based on combined scores across documentation quality, technical infrastructure, and health & sustainability. Official designations were further validated against live GitHub metrics and internal context from subject matter reviewers.

The final distribution of repositories across maturity phases is as follows:

| Maturity Phase | Description                                                                                                   | # of Projects | % of Total |
| -------------- | ------------------------------------------------------------------------------------------------------------- | ------------- | ---------- |
| Mature         | Fully stable, with comprehensive documentation, sound engineering, and governance, minor room for improvement | 32            | 48.5%      |
| Growth         | Actively developed with increasing structure and community engagement, room for improvement                   | 13            | 19.7%      |
| Maintenance    | Stable and functional, but with minimal new development activity                                              | 14            | 21.2%      |
| Incubation     | Early stage, limited contributors or formal documentation, major room for improvement                         | 7             | 10.6%      |

Note: No repositories were officially designated as “Decline” or “Archived” in the current dataset, although some repositories scored near thresholds that could indicate future deprecation risk.

#### Key Observations:

* Mature repositories represent nearly half of the portfolio and tend to have active CI/CD, comprehensive test coverage, documented governance, and high community signals (stars, forks, issues). These are excellent candidates for showcasing externally or adopting as long-term maintained assets.
* Growth-phase projects demonstrated strong activity but often lacked formal governance or complete documentation. These represent high-leverage opportunities where small investments (like CONTRIBUTING files or release processes) can accelerate maturity.
* Maintenance-phase repositories showed signs of long-term use but limited ongoing contributions. Many are functionally complete or serve niche legacy roles. These should be monitored to ensure security hygiene and tagged accordingly for downstream consumers.
* Incubation-phase projects are largely in early development or were recently open-sourced. Most lacked full setup documentation, test automation, or active contributors. These require clearer ownership and development plans if they are to mature effectively.

4\. Detailed Results:

| Repo Name                        | Repo Link                                                                                                                                     | Official Maturity Rating | Overall Scoring | Tech Maturity | Health maturity | Doc Maturity |   |
| -------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ | --------------- | ------------- | --------------- | ------------ | - |
| .github                          | [https://github.com/IntersectMBO/.github](https://github.com/IntersectMBO/.github)                                                            | Maintenance              | 16              | Incubation    | Healthy 🟢      | Incubation   |   |
| antaeus                          | [https://github.com/IntersectMBO/antaeus](https://github.com/IntersectMBO/antaeus)                                                            | Mature                   | 28              | Growth        | Moderate 🟡     | Mature       |   |
| bech32                           | [https://github.com/IntersectMBO/bech32](https://github.com/IntersectMBO/bech32)                                                              | Mature                   | 29              | Growth        | Healthy 🟢      | Mature       |   |
| budget-documentation             | [https://github.com/IntersectMBO/budget-documentation](https://github.com/IntersectMBO/budget-documentation)                                  | Maintenance              | 25              | Incubation    | Healthy 🟢      | Mature       |   |
| cardaminal                       | [https://github.com/IntersectMBO/cardaminal](https://github.com/IntersectMBO/cardaminal)                                                      | Mature                   | 32              | Growth        | Healthy 🟢      | Mature       |   |
| cardano-addresses                | [https://github.com/IntersectMBO/cardano-addresses](https://github.com/IntersectMBO/cardano-addresses)                                        | Mature                   | 31.5            | Growth        | Healthy 🟢      | Mature       |   |
| cardano-airgap                   | [https://github.com/IntersectMBO/cardano-airgap](https://github.com/IntersectMBO/cardano-airgap)                                              | Mature                   | 24.5            | Incubation    | Moderate 🟡     | Mature       |   |
| cardano-api                      | [https://github.com/IntersectMBO/cardano-api](https://github.com/IntersectMBO/cardano-api)                                                    | Mature                   | 32.5            | Growth        | Healthy 🟢      | Mature       |   |
| cardano-base                     | [https://github.com/IntersectMBO/cardano-base](https://github.com/IntersectMBO/cardano-base)                                                  | Mature                   | 33.5            | Growth        | Healthy 🟢      | Mature       |   |
| cardano-cli                      | [https://github.com/IntersectMBO/cardano-cli](https://github.com/IntersectMBO/cardano-cli)                                                    | Mature                   | 32              | Growth        | Healthy 🟢      | Mature       |   |
| cardano-coin-selection           | [https://github.com/IntersectMBO/cardano-coin-selection](https://github.com/IntersectMBO/cardano-coin-selection)                              | Mature                   | 25.5            | Incubation    | Healthy 🟢      | Mature       |   |
| cardano-crypto                   | [https://github.com/IntersectMBO/cardano-crypto](https://github.com/IntersectMBO/cardano-crypto)                                              | Mature                   | 25.5            | Growth        | Moderate 🟡     | Mature       |   |
| cardano-db-sync                  | [https://github.com/IntersectMBO/cardano-db-sync](https://github.com/IntersectMBO/cardano-db-sync)                                            | Mature                   | 30.5            | Growth        | Moderate 🟡     | Mature       |   |
| cardano-haskell-packages         | [https://github.com/IntersectMBO/cardano-haskell-packages](https://github.com/IntersectMBO/cardano-haskell-packages)                          | Growth                   | 22              | Growth        | Moderate 🟡     | Mature       |   |
| cardano-launcher                 | [https://github.com/IntersectMBO/cardano-launcher](https://github.com/IntersectMBO/cardano-launcher)                                          | Mature                   | 33              | Growth        | Healthy 🟢      | Mature       |   |
| cardano-ledger                   | [https://github.com/IntersectMBO/cardano-ledger](https://github.com/IntersectMBO/cardano-ledger)                                              | Mature                   | 35              | Growth        | Healthy 🟢      | Mature       |   |
| cardano-node                     | [https://github.com/IntersectMBO/cardano-node](https://github.com/IntersectMBO/cardano-node)                                                  | Mature                   | 31.5            | Growth        | Moderate 🟡     | Mature       |   |
| cardano-node-emulator            | [https://github.com/IntersectMBO/cardano-node-emulator](https://github.com/IntersectMBO/cardano-node-emulator)                                | Mature                   | 30.5            | Incubation    | Healthy 🟢      | Mature       |   |
| cardano-node-tests               | [https://github.com/IntersectMBO/cardano-node-tests](https://github.com/IntersectMBO/cardano-node-tests)                                      | Mature                   | 28              | Growth        | Moderate 🟡     | Mature       |   |
| cardano-prelude                  | [https://github.com/IntersectMBO/cardano-prelude](https://github.com/IntersectMBO/cardano-prelude)                                            | Growth                   | 20.5            | Growth        | Unhealthy 🔴    | Mature       |   |
| cardano-sync-tests               | [https://github.com/IntersectMBO/cardano-sync-tests](https://github.com/IntersectMBO/cardano-sync-tests)                                      | Incubation               | 9               | Incubation    | Moderate 🟡     | Archive      |   |
| cardano-test-plans               | [https://github.com/IntersectMBO/cardano-test-plans](https://github.com/IntersectMBO/cardano-test-plans)                                      | Growth                   | 20              | Incubation    | Healthy 🟢      | Archive      |   |
| cardano-transactions             | [https://github.com/IntersectMBO/cardano-transactions](https://github.com/IntersectMBO/cardano-transactions)                                  | Mature                   | 28.5            | Incubation    | Healthy 🟢      | Mature       |   |
| cardano-updates                  | [https://github.com/IntersectMBO/cardano-updates](https://github.com/IntersectMBO/cardano-updates)                                            | Growth                   | 20              | Growth        | Moderate 🟡     | Mature       |   |
| cardano-world                    | [https://github.com/IntersectMBO/cardano-world](https://github.com/IntersectMBO/cardano-world)                                                | Mature                   | 27              | Growth        | Healthy 🟢      | Mature       |   |
| cc-portal                        | [https://github.com/IntersectMBO/cc-portal](https://github.com/IntersectMBO/cc-portal)                                                        | Mature                   | 30              | Growth        | Healthy 🟢      | Mature       |   |
| civics-documentation             | [https://github.com/IntersectMBO/civics-documentation](https://github.com/IntersectMBO/civics-documentation)                                  | Maintenance              | 28              | Incubation    | Healthy 🟢      | Mature       |   |
| committees-groups-documentation  | [https://github.com/IntersectMBO/committees-groups-documentation](https://github.com/IntersectMBO/committees-groups-documentation)            | Maintenance              | 25              | Growth        | Moderate 🟡     | Mature       |   |
| credential-manager               | [https://github.com/IntersectMBO/credential-manager](https://github.com/IntersectMBO/credential-manager)                                      | Mature                   | 29              | Growth        | Healthy 🟢      | Mature       |   |
| developer-experience             | [https://github.com/IntersectMBO/developer-experience](https://github.com/IntersectMBO/developer-experience)                                  | Growth                   | 23              | Incubation    | Moderate 🟡     | Mature       |   |
| drep-campaign-platform           | [https://github.com/IntersectMBO/drep-campaign-platform](https://github.com/IntersectMBO/drep-campaign-platform)                              | Growth                   | 22              | Incubation    | Healthy 🟢      | Mature       |   |
| drep-code-of-conduct             | [https://github.com/IntersectMBO/drep-code-of-conduct](https://github.com/IntersectMBO/drep-code-of-conduct)                                  | Mature                   | 24              | Incubation    | Healthy 🟢      | Growth       |   |
| essential-cardano                | [https://github.com/IntersectMBO/essential-cardano](https://github.com/IntersectMBO/essential-cardano)                                        | Growth                   | 20              | Growth        | Moderate 🟡     | Mature       |   |
| formal-ledger-specifications     | [https://github.com/IntersectMBO/formal-ledger-specifications](https://github.com/IntersectMBO/formal-ledger-specifications)                  | Mature                   | 27.5            | Growth        | Healthy 🟢      | Mature       |   |
| governance-actions               | [https://github.com/IntersectMBO/governance-actions](https://github.com/IntersectMBO/governance-actions)                                      | Growth                   | 16.5            | Incubation    | Moderate 🟡     | Growth       |   |
| governance-tools-documentation   | [https://github.com/IntersectMBO/governance-tools-documentation](https://github.com/IntersectMBO/governance-tools-documentation)              | Mature                   | 20.5            | Growth        | Unhealthy 🔴    | Mature       |   |
| govtool                          | [https://github.com/IntersectMBO/govtool](https://github.com/IntersectMBO/govtool)                                                            | Mature                   | 30              | Growth        | Moderate 🟡     | Mature       |   |
| govtool-delegation-pillar        | [https://github.com/IntersectMBO/govtool-delegation-pillar](https://github.com/IntersectMBO/govtool-delegation-pillar)                        | Mature                   | 26.5            | Incubation    | Healthy 🟢      | Mature       |   |
| govtool-outcomes-pillar          | [https://github.com/IntersectMBO/govtool-outcomes-pillar](https://github.com/IntersectMBO/Win32-network)                                      | Growth                   | 20.5            | Incubation    | Moderate 🟡     | Mature       |   |
| govtool-proposal-discussion      | [https://github.com/IntersectMBO/govtool-proposal-discussion](https://github.com/IntersectMBO/govtool-proposal-discussion)                    | Mature                   | 24              | Incubation    | Healthy 🟢      | Mature       |   |
| govtool-proposal-pillar          | [https://github.com/IntersectMBO/govtool-proposal-pillar](https://github.com/IntersectMBO/govtool-proposal-pillar)                            | Mature                   | 27              | Growth        | Moderate 🟡     | Mature       |   |
| govtool-test-reports             | [https://github.com/IntersectMBO/govtool-test-reports](https://github.com/IntersectMBO/govtool-test-reports)                                  | Incubation               | 12.5            | Maintenance   | Moderate 🟡     | Incubation   |   |
| govtool-voting-pillar            | [https://github.com/IntersectMBO/govtool-voting-pillar](https://github.com/IntersectMBO/govtool-voting-pillar)                                | Mature                   | 24              | Growth        | Moderate 🟡     | Mature       |   |
| hf-wg-documentation              | [IntersectMBO/hf-wg-documentation: Repository for hardfork working group documentation.](https://github.com/IntersectMBO/hf-wg-documentation) | Maintenance              | 19.5            | Growth        | Moderate 🟡     | Incubation   |   |
| intersect-constitutional-council | [https://github.com/IntersectMBO/intersect-constitutional-council](https://github.com/IntersectMBO/intersect-constitutional-council)          | Growth                   | 16.5            | Incubation    | Moderate 🟡     | Growth       |   |
| intersect-knowledge-base         | [https://github.com/IntersectMBO/intersect-knowledge-base](https://github.com/IntersectMBO/intersect-knowledge-base)                          | Maintenance              | 28.5            | Incubation    | Healthy 🟢      | Mature       |   |
| intersect-landscape              | [https://github.com/IntersectMBO/intersect-landscape](https://github.com/IntersectMBO/intersect-landscape)                                    | Growth                   | 17              | Growth        | Moderate 🟡     | Archive      |   |
| intersect-steering-documentation | [https://github.com/IntersectMBO/intersect-steering-documentation](https://github.com/IntersectMBO/intersect-steering-documentation)          | Maintenance              | 23              | Growth        | Unhealthy 🔴    | Mature       |   |
| io-classes-extra                 | [IntersectMBO/io-classes-extra: Utilities built on top of \`io-classes\`](https://github.com/IntersectMBO/io-classes-extra)                   | Growth                   | 15              | Incubation    | Moderate 🟡     | Incubation   |   |
| libsodium                        | [https://github.com/IntersectMBO/libsodium](https://github.com/IntersectMBO/libsodium)                                                        | Maintenance              | 12              | Incubation    | Moderate 🟡     | Mature       |   |
| lsm-tree                         | [https://github.com/IntersectMBO/lsm-tree](https://github.com/IntersectMBO/lsm-tree)                                                          | Mature                   | 28              | Growth        | Moderate 🟡     | Mature       |   |
| mcc-documentation                | [https://github.com/IntersectMBO/mcc-documentation](https://github.com/IntersectMBO/mcc-documentation)                                        | Maintenance              | 26              | Growth        | Moderate 🟡     | Mature       |   |
| nami                             | [https://github.com/IntersectMBO/nami](https://github.com/IntersectMBO/nami)                                                                  | Mature                   | 31.5            | Growth        | Healthy 🟢      | Incubation   |   |
| open-source-office               | [https://github.com/IntersectMBO/open-source-office](https://github.com/IntersectMBO/open-source-office)                                      | Maintenance              | 29              | Growth        | Healthy 🟢      | Mature       |   |
| osc-documentation                | [https://github.com/IntersectMBO/osc-documentation](https://github.com/IntersectMBO/osc-documentation)                                        | Maintenance              | 27              | Growth        | Healthy 🟢      | Mature       |   |
| ouroboros-consensus              | [https://github.com/IntersectMBO/ouroboros-consensus](https://github.com/IntersectMBO/ouroboros-consensus)                                    | Mature                   | 34.5            | Growth        | Healthy 🟢      | Mature       |   |
| ouroboros-network                | [https://github.com/IntersectMBO/ouroboros-network](https://github.com/IntersectMBO/ouroboros-network)                                        | Mature                   | 33.5            | Growth        | Healthy 🟢      | Mature       |   |
| parameters-documentation         | [https://github.com/IntersectMBO/parameters-documentation](https://github.com/IntersectMBO/parameters-documentation)                          | Maintenance              | 29.5            | Incubation    | Healthy 🟢      | Mature       |   |
| pdf-ui                           | [https://github.com/IntersectMBO/pdf-ui](https://github.com/IntersectMBO/pdf-ui)                                                              | Growth                   | 23.5            | Growth        | Healthy 🟢      | Archive      |   |
| plutus                           | [https://github.com/IntersectMBO/plutus](https://github.com/IntersectMBO/plutus)                                                              | Mature                   | 34.5            | Growth        | Healthy 🟢      | Mature       |   |
| plutus-script-evaluation         | [https://github.com/IntersectMBO/plutus-script-evaluation](https://github.com/IntersectMBO/plutus-script-evaluation)                          | Incubation               | 17              | Incubation    | Healthy 🟢      | Archive      |   |
| plutus-tx-template               | [https://github.com/IntersectMBO/plutus-tx-template](https://github.com/IntersectMBO/plutus-tx-template)                                      | Incubation               | 28.5            | Incubation    | Healthy 🟢      | Mature       |   |
| product-documentation            | [https://github.com/IntersectMBO/product-documentation](https://github.com/IntersectMBO/product-documentation)                                | Maintenance              | 29              | Incubation    | Healthy 🟢      | Mature       |   |
| tsc-documentation                | [https://github.com/IntersectMBO/tsc-documentation](https://github.com/IntersectMBO/tsc-documentation)                                        | Maintenance              | 21.5            | Incubation    | Moderate 🟡     | Mature       |   |
| win32-network                    | [https://github.com/IntersectMBO/Win32-network](https://github.com/IntersectMBO/Win32-network)                                                | Incubation               | 22              | Incubation    | Healthy 🟢      | Mature       |   |
| workgroup-info                   | [https://github.com/IntersectMBO/workgroup-info](https://github.com/IntersectMBO/Win32-network)                                               | Incubation               | 19              | Incubation    | Healthy 🟢      | Mature       |   |

### Source Documents:

{% embed url="https://docs.google.com/spreadsheets/d/1XOeNnmBCn-umkTDksKm7Secb4Pp2oEICPfC-DdXj4a4/edit?usp=sharing" %}

{% file src=".gitbook/assets/2025 Project Lifecycle Maturity Tiers V1.0 (2).pdf" %}
