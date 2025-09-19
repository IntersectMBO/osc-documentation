---
description: >-
  This is a working draft. Nothing here should be treated as final until
  formally approved. Formal OSC approval to follow.
---

# 🫣 Incident Monitoring

### **Executive Summary:**

As steward of the Haskell Core Node Repositories and a coordination point for decentralized projects, Intersect MBO is establishing a **decentralized security support process** that plugs into existing stakeholder setups—SPO networks, core engineering teams, vendors, community ops, and the Security Council/technical committees. The goal is a coordinated, accountable approach to issues affecting core node operations and broader ecosystem incidents.\
**The process aims to:**

* **Unify intake & triage:** Provide a single, coordinated path for reports (vulnerabilities, outages, anomalies) with a shared severity model and escalation map; ideally avoiding ad-hoc routes that slow response or miss critical reviewers.
* **Activate the right people fast:** Use pre-agreed bridges to SPOs, core teams, wallet/providers, infra hosts, and community leads; ideally so there’s no guessing about ownership or next steps.
* **Standardize communications:** Deliver role-specific updates (operators, developers, community) to ideally minimize misinformation and conflicting guidance.
* **Share tooling & signals:** Pool monitoring (network health, transaction/contract/wallet tracking, alerts) to ideally reduce blind spots and duplication.
* **Build durable muscle memory:** Run common playbooks, on-call rotations, and cross-org drills so responses are repeatable; not personality or team dependent.
* **Ensure sustainability & reliability:** Define clear RACI and run post-incident reviews that feed into governance and secure SDLC for continuous improvement.

**Bottom line:** A decentralized, community-coordinated process replaces today’s fragmented, siloed efforts with a **reliable, ecosystem-wide response system** for faster, clearer, and more trustworthy for everyone.

### How This Works

#### Coordination Layer

The **Security Council (SC)** serves as the coordination layer for decentralized security support Haskell Node. It assesses risks, validates incidents, and determines the appropriate response under the Incident Management Process. The SC ensures governance continuity while drawing on additional support from the **Open Source Committee (OSC)** and the **Technical Steering Committee (TSC)** to align technical and governance actions across the landscape.

#### Operational Lead: Security Incident Officer (SIO)

To operationalize this mandate, the SC will onboard a **Security Incident Officer (SIO)** who acts as the first responder and day-to-day lead for intake, triage, and orchestration. The SIO receives **direct support from the Open Source Office (OSO) team** within Intersect, ensuring resources, coordination capacity, and continuity across projects.

Core responsibilities of the SIO include:

* **First response & triage** – intake of reports, severity classification, and escalation.
* **Monitoring & detection** – observing Cardano network health, developer and social channels, and system telemetry.
* **Risk register management** – maintaining an ecosystem-wide vulnerability/risk log.
* **Cross-community coordination** – engaging SPOs, core teams, vendors, and infra providers.
* **Stakeholder communications** – tailoring updates for developers, operators, and the wider community.
* **Procedure development & drills** – defining playbooks and running exercises.
* **Release event oversight** – monitoring critical software releases to ensure secure deployment.
* **Best practices adoption** – embedding CI/CD checks, static analysis, and security scanning into repos.
* **Tooling feasibility** – designing/assessing monitoring solutions (transactions, contracts, wallets, addresses, dashboards, alerts)

#### External Coordination with Partner IR Teams

The SIO will work closely with **partner incident-response providers** such as the Cardano Foundation and Input Output. This collaboration ensures:

* Pre-agreed escalation bridges and secure comms.
* Shared severity classification and coordinated timelines.
* Joint triage and mitigation efforts across organizations.
* Aligned public communications to avoid contradictory messaging.
* Joint post-incident reviews feeding into updated playbooks and monitoring.

#### Broader Support Roles

* The **Open Source Office (OSO)** provides program management, administrative, and operational support to the SIO, ensuring consistent follow-through and documentation.
* The **OSC and TSC** provide additional operational and subject-matter expertise to the SC, backing up decision-making with governance alignment and technical validation.



### Job Description for the Security Incident Officer:

| Department:   | Open Source Office and (Security Council) |
| ------------- | ----------------------------------------- |
| Job Function: | Security Incident Officer                 |

Department:\
Open Source Office (OSO) – Intersect MBO

Job Function:\
Incident Security Officer on 12 Month Contract

Salary Range: Tied to the [approved treasury action](https://gov.tools/outcomes/governance_actions/8ad3d454f3496a35cb0d07b0fd32f687f66338b7d60e787fc0a22939e5d8833e#11) a salary equivalent of $70,000–$80,000 USD, adjusted to local currency based on experience.

Summary\
At Intersect, a member-led organization supporting Cardano’s decentralized governance, open-source technology, and long-term resilience, we are seeking an experienced Security Incident Officer to drive the evaluation and development of security process offerings across our organization interfacing to the Cardano blockchain.  Reporting to the Head of the Open Source Office and forging close working relationships with the Security Council and technical committees at Intersect, this role will coordinate incident response procedures, engage with developers and community stakeholders, and support network resilience through monitoring, facilitating response drills, and secure software practices.

This is a key role for someone passionate about decentralization, blockchain analysis and security. You will work closely with our members across the Security Council, Technical Steering Committee, and Open Source Committee to evaluate and implement the initial stages of decentralized security tooling and processes on behalf of the MBO. &#x20;

Duties:\


* First response and triage. Serve as a public contact for reported security incidents and potential vulnerabilities across the Cardano blockchain and tooling. Expect to be regularly on-call on a rotating basis with other first responders.
* Monitoring and detection. Track and report on available signals relating to the Cardano network, social media, and developer channels for signs of breaches, proposed attacks, or newly discovered vulnerabilities.
* Risk register maintenance. Support efforts to establish and maintain a community risk and vulnerability register -  contributing to timely updates and accurate classification of risks.
* Community coordination. Coordinate cross-functional response efforts by engaging stake pool operators (SPOs), developers, and other stakeholders to support timely and effective mitigation.
* Stakeholder communication. Coordinate clear, discreet, and reassuring information flows to community members, developer organizations, and other key stakeholders.
* Procedure development. Define, document, and manage incident response procedures. Support network resilience by facilitating response exercises and encouraging secure software practices.
* Release event oversight. Monitor major releases and manage critical incident processes around them to help facilitate secure deployment and risk mitigation.
* Adoption of best practices. Recommend and coordinate static analysis and CI practices across Intersect-managed codebases.
* Tooling Monitoring. Feasibility, outline design, constraints and indicative costs for an internal chain monitoring solution. Feasibility assessment  should include services such as;
  * Transaction monitoring
  * Smart Contract monitoring
  * Wallet and Address tracking
  * Network Health monitoring
  * Analytics & Dashboards
  * Real-Time Alerts & Notifications

Key Competencies

* Calm, reassuring presence in high-pressure situations.
* Strong coordination skills to align technical teams during time-critical incidents.
* Discretion and professionalism in handling sensitive security information.
* Ability to communicate clearly with stakeholders concerned about risk to their capital.
* Strong organizational skills to manage simultaneous incidents, drills, and processes.

Education / Experience

* Proven experience in incident management and response.
* Background in project coordination, ideally with globally distributed teams.
* Knowledge of code security practices, including CI/CD pipelines, vulnerability scanners, and static analysis tooling.
* Expertise in observability tools and practices (e.g. log analysis, metrics, graphing tools and services like Grafana, Prometheus…).
* Experience working with open-source projects or blockchain ecosystems preferred.
* Familiarity with Cardano Core Node Tech Stack (Node, Govtool, Plutus, etc)
