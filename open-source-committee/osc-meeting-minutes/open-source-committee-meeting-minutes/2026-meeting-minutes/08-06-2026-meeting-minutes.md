# (08/06/2026) Meeting Minutes

## Attendees:&#x20;

| Name                     | Attendance | Role       | Voting Seat (Y/N) | Term            |
| ------------------------ | ---------- | ---------- | ----------------- | --------------- |
| Sebastian Pabon          | Yes        | Chair      | Y                 | October 2025    |
| Kambale Mechack Elie     | Yes        | Vice Chair | Y                 | April 2026 (2y) |
| Terence ‘Tex’ McCutcheon | Yes        | Secretary  | N                 | N/A             |
| Bernard Sibanda          | Yes        | Member     | Y                 | October 2025    |
| Jordan Hill              | No         | Member     | Y                 | October 2025    |
| Udai Solanki             | Yes        | Member     | Y                 | October 2025    |
| Reshma Mohan             | Yes        | Member     | Y                 | October 2025    |
| Pawel Jakubas            | No         | Member     | Y                 | April 2026 (2y) |
| Olivier Mwatsimulamo     | No         | Member     | Y                 | April 2026 (2y) |
| Bora Oben                | Yes        | Member     | Y                 | April 2026 (2y) |
| Dominik Hinkleman        | No         | Member     | Y                 | April 2026 (2y) |

Community/Other Attendees

* Adam Dean
* Adam Rusch
* Darlington Wleh
* Emmanuel Titi
* Mathieu Montin



**Recording:** [Open Source Committee (Intersect) - 2026/08/06 - Recording](https://drive.google.com/file/d/1evLnj7_kcGdYRb4-DmSRVpyyIxj-2m1Q/view?usp=sharing)

**Transcript:** [Open Source Committee (Intersect) - 2026/08/06 - Transcript](https://docs.google.com/document/d/1sUSLJatOD7RckurEDYrvTT5wbWl3xI4aSMKEj_qyqm0/edit?usp=sharing)

**Chat Transcript:** [Open Source Committee Meeting – 2026/08/06 – Chat Transcript](https://drive.google.com/file/d/1H597tNivUFoAYL3e-mLQpS1HMHQgjz0Z/view?usp=sharing)

## Intros

**Bora:** TBD\
**Bernard:** OSC - voting member\
**Dominik:** Open Source Committee Member, part of Inferara.\
**Jordan:** TBD\
**Kambale:** OSC Vice chair\
**Olivier:** Goma Hub Member, Milestone Reviewer-Project Catalyst, MCC and OSC\
**Pawel:** Member OSC, CF\
**Reshma:** OSC voting member\
**Sebastian:** OSC chair. Andamio co-founder.\
**Tex:** Open Source Program Manager, Intersect, OSC Secretary, Committee Member Advocate\
**Udai:** Member OSC, AIQUANT Technologies

## Agenda 8.06.26

* MRP Status Updates
* Cella SoW
* CNE SoW
* DB-Sync Website
* Ekklesia Stack Development
* Regulatory Evidence Portal (Tooling Proposal)
* Developer Advocate Program - Closeout Docs
* MRP Interview Document
* Discord/Async Communication
* 2025 Treasury Withdrawal Budget Awareness
* Vantage Report - Guidelines Draft
* Open Forum

## Decisions/Actions

**Decisions**

* **No Formal Committee Decisions Were Approved:** Due to the absence of a quorum (only 5 of 9 voting committee members were present), the Open Source Committee was unable to pass any official binding decisions during the meeting.
* **Cardano Node Emulator SoW Status:** A previous asynchronous vote in the committee's Discord channel resulted in a 3-3 tie; therefore, the proposal remains formally unapproved and open for further discussion/re-voting.

**Actions**

**Terence:**

* Post a series of asynchronous polls/votes in the OSC Discord channel for the Maintainer Retainer Program (MRP) updates (including Adam Dean's assignment), the Chella Statement of Work (SoW), and the Cardano Node Emulator SoW.
* Check past meeting minutes to verify previous SoW approvals and review process details.
* Coordinate with Darlington regarding hosting capabilities, GitLab action permissions, and subdomain requirements for the proposed DBSync documentation site.
* Schedule a follow-up conversation with Bora and Adam Rusch to further discuss ecosystem tooling mapping and the Regulatory Evidence Portal.
* Publish the final meeting minutes to the committee.

**Darlington & Bora:**

* Connect asynchronously with Matthieu (Pizenberg) regarding CIP-179 to explore using on-chain polling mechanisms for the proposed DBSync user survey instead of a custom Cloudflare/SQLite back end.

**Committee Members (All):**

* Review and leave feedback/comments on the Cella SoW and the Cardano Node Emulator SoW.
* Review Adam Rusch’s report and proof-of-concept for the Regulatory Evidence Portal and submit feedback/questions ahead of the next discussion.
* Engage in upcoming Discord polls to help reach quorum asynchronously on pending agenda items.

| Topic                                       | Discussion                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Notes                                                                                                                                                                                                                                |
| ------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Meeting Opening & Quorum                    | Terence opened the meeting and noted that quorum was not yet met with only five committee members present out of nine. Discussions proceeded while waiting for potential late arrivals.                                                                                                                                                                                                                                                                    | Attendees and committee members introduced themselves; Sebastian (Chair) was present.                                                                                                                                                |
| Maintainer Retainer Program (MRP) Updates   | Terence shared that the Maintainer Retainer Program is fully underway with months 1–4 available for original maintainers. Updates were provided on recent interviews, candidate reviews, and proposed assignments.                                                                                                                                                                                                                                         | <p>• Exploring options with TX Pipe.<br>• Proposed assigning Adam (Dean) to the Ekklesia voting stack.<br>• Requests made for spots for DQuadrant (GovTool) and Adam (Rusch).</p>                                                    |
| Cella Statement of Work (SoW)               | Terence provided the Cella SoW in Google Doc format for review. No comments had been submitted yet, and feedback is needed before moving to the contracting phase.                                                                                                                                                                                                                                                                                         | Terence refreshed and re-shared the Cella document link in the Discord channel.                                                                                                                                                      |
| Cardano Node Emulator SoW & Tooling Debates | Udai noted previous approval for SoW submission, but Terence clarified that formal SoW approval requires a committee vote. A prior Discord vote resulted in a 3-3 tie. Bora detailed concerns about high costs and existing alternative tooling (e.g., evolution, mesh) serving local developer testnets. Mathieu explained the intent to revamp the tool before handing it to a community maintainer and noted flexibility regarding the budget/timeline. | <p>• Budget and overlap with broader SDK/off-chain tools were the main points of debate.<br>• Proposer Mathieu was praised for transparency regarding current low traction.<br>• Re-voting will occur asynchronously in Discord.</p> |
| DBSync Website & Config Builder Proposal    | Darlington presented a proposal for a dedicated DBSync static documentation site (built with Docusaurus/React) featuring a config builder, compute/memory projection tools, example queries, and a usage survey.                                                                                                                                                                                                                                           | <p>• Intersect support needed for hosting, GitLab actions, and a subdomain.<br>• Bora suggested leveraging CIP-179 for on-chain polling to eliminate back-end infrastructure.</p>                                                    |
| Ecclesia Voting Stack Integration           | Adam (Dean) delivered an elevator pitch to bring the Ekklesia Development Fund under Intersect as a sub-organization (similar to the CNCF model). The stack uses Hydra L2 state channels for zero-cost community polling and avoids creating long-term financial burdens on Intersect.                                                                                                                                                                     | <p>• Intersect would provide non-profit umbrella oversight and budget administration.<br>• The Open Source Committee (OSC) would handle high-level governance and dispute arbitration.</p>                                           |
| Cella vs. Ecclesia Scope Clarification      | Udai inquired whether there was functional overlap between Cella and Ekklesia. Terence and Adam clarified their distinct scopes: Cella is tailored for Constitutional Committee multi-sig votes, whereas Ekklesia is aimed at lightweight, general ecosystem polling for wallet holders and DReps.                                                                                                                                                         | The tools address different governance layers and remain independent initiatives.                                                                                                                                                    |
| Regulatory Evidence Portal Proposal         | Adam (Rusch) presented a proof-of-concept portal designed to gather on-chain metrics and generate daily cryptographic hashes to show regulators (e.g., under the US Clarity Act) that Cardano is a mature, decentralized blockchain system.                                                                                                                                                                                                                | <p>• Seeking a developer/maintainer to audit the code base and help launch on Intersect infrastructure.<br>• Estimated cost: $15,000–$20,000 for one year, including $3,000–$5,000 for a code audit.</p>                             |
| Data Aggregation & Alternatives Discussion  | Bora questioned whether existing abstractions like Dune Analytics or Yaci Store could serve these regulatory metrics without building custom tools. Adam (Rusch) and Adam (Dean) emphasized the importance of self-hosted, dedicated evidence chains over third-party licensed platforms.                                                                                                                                                                  | Adam (Rusch) highlighted the strategic urgency of establishing an evidence record ahead of upcoming legislative decisions.                                                                                                           |
| Ecosystem Mapping & Async Communication     | Terence suggested for Bora to create an ecosystem tooling map to help the committee identify existing solutions prior to public meetings. He also noted the need to improve asynchronous communication and decision-making on Discord.                                                                                                                                                                                                                     | Follow-up discussions and asynchronous polls will be posted in Discord.                                                                                                                                                              |
