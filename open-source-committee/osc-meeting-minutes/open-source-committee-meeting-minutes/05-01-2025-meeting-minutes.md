# 🙃 (05/01/2025) Meeting Minutes

## Attendees:&#x20;

| Name                     | Attendance | Role        | Voting Seat (Y/N) |
| ------------------------ | ---------- | ----------- | ----------------- |
| P. Lucas                 | Yes        | Chair       | Y                 |
| Adam Dean                | Yes        | Vice Chair  | Y                 |
| Terence ‘Tex’ McCutcheon | Yes        | Secretary   | N                 |
| Christian Taylor         | Yes        | Member/Seat | N                 |
| Sandip Pandey            | Yes        | Member/Seat | Y                 |
| Georg Link               | Yes        | Member/Seat | Y                 |
| Jonathan Kelly           | Yes        | Member/Seat | Y                 |
| Sebastian Pabon          | No         | Member/Seat | Y                 |
| Moritz Angermann         | No         | Member/Seat | Y                 |
| Robin Böning             | No         | Member/Seat | Y                 |
| Nicolas Henin            | No         | Member/Seat | Y                 |

Community/Other Attendees

* Alex Seregin
* Georgia Hutton
* Jordan Hill

**Recording:** [Open Source Committee (Intersect) - 2025/05/01 - Recording](https://drive.google.com/file/d/16poBRtTYm3lPs-XhT-7t86j26uTOqttT/view?usp=sharing)

**Transcript:** [Open Source Committee (Intersect) - 2025/05/01 - Transcript](https://docs.google.com/document/d/1ZTUm8XGqVh8mij0boLoXQO4lqx9NNbgismS4kmVea9o/edit?usp=sharing)

**Chat Transcript:** [Open Source Committee Meeting – 2025/05/01 – Chat Transcript](https://drive.google.com/file/d/1CBs1Nk1vDG1C4Nc4N7Eq_wrHq2kTJcpE/view?usp=sharing)

## Intros

**Christian:** Head of Open Source Office, Intersect Staff

**Tex:** Open Source Program Manager, Intersect Staff, Open Source Committee Secretary

**Sandip:** Dquadrant

**Adam:** Adam Dean, LLC, Co-Founder, DripDropz, LLC, CIP Editors, Intersect Maintainer

**Georg:** Bitergia

**Lucas:** 45B - Cardano Enablement, Onboarding end-users; Supporting cardano Projects;

**Sebastian:** Gimbalabs contributor, MeshJS contributor, Andamio platform co-founder

**Johnny:** Non-Custodial Co-Management SysOps Engineer (Tech Janitor) for 3 Mainnet Stake Pools. Cardano Keystone Wallet Ambassador.

**Moritz:** Head of Platform Engineering, IOE&#x20;

**Nicolas:** Technical Architect at IOG (Innovation R\&D)&#x20;

**Robin:** Cardano Cube, LACE stake pool

## Agenda 5.1.25

* Old Business
  * Committee Member Engagement
* New Business
  * OS Strategy Revisions
  * Backend Budget Process Discussion
  * KES Repo Migration

## Decisions/Actions

* **Agenda Rearrangement:** A decision was made to move the budget management discussion to the front of the agenda to accommodate Georgia's presence.
* **Deferral of Strategy Rework:** The committee agreed to defer the rework of the OSC strategy document until the new committee members are onboarded and the budget is finalized.
* **Onboarding Process and Chair Selection Deferral:** The committee approved Pedro's proposed plan for onboarding new members, which includes hosting a separate onboarding call outside of regular meetings and deferring the selection or vote for a new chair until at least the third call after onboarding.

| Topic                                         | Discussion                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Action Items                                                                                                                                                                                                                                                                                                           |
| --------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Meeting Opening & Agenda Review               | Terence welcomed attendees. Agenda was reviewed, including committee member actions, separate workspace meetings, and onboarding document. Decision made to move budget management discussion forward due to Georgia's presence.                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Committee members to review the onboarding document.                                                                                                                                                                                                                                                                   |
| Budget Management & Prioritization            | Georgia (Intersect) explained the need to start prioritizing budget items as the proposal is expected to pass soon, with funds available around 12 weeks post-withdrawal. Discussed planning for procurement, grant-style applications, and events. Christian provided initial thoughts on prioritizing programs: Developer Advocates (easy win, existing template), Maintainer Retainer (qualification criteria, contract template), Tooling Sustainability (similar review), Bug Bounty, Incident Monitoring, Code for Us, Accelerator Research Program. Pedro suggested starting with low-hanging fruit (Dev Advocate, Bug Bounty) and deferring others (Accelerator Research).                             | Committee to discuss and prioritize budget items/programs based on the proposal. Pedro to share screen with the budget proposal for discussion. Christian to follow up with Chris Kowalsski regarding the Accelerator Research Program operationalization plan.                                                        |
| Funds Operational Workflow                    | Terence inquired about the process for fund disbursement (via CDH/Intersect contracts vs. multi-sig wallet). Georgia stated this is under discussion internally and an update would be provided soon. Jonathan requested a standard operating procedure (SOP) for funds workflow across committees, expressing concern about ad hoc processes and the risk of funds being locked or lost.                                                                                                                                                                                                                                                                                                                      | Georgia (or Intersect) to provide an update on the funds operational flow and SOP as soon as information is available.                                                                                                                                                                                                 |
| KYC/KYB Process for Contracts/Grants          | Question raised if every tooling provider/maintainer requires Intersect KYC/KYB. Georgia confirmed this has been standard practice for contracts (Dev Advocates were KYC'd). Adam mentioned potential country restrictions based on US law. Terence proposed making KYC voluntary and integrated into a website check system. Georgia noted current system uses unique links but could be explored. Christian asked about KYC for Bug Bounty payments.                                                                                                                                                                                                                                                         | Georgia (or Intersect ops channel) to confirm specific KYB/KYC requirements and process details for various programs (e.g., Bug Bounty). Terence to explore options for website integration of voluntary KYC/KYB with relevant teams. Christian to seek input from Foundation contacts on KYC for Bug Bounty payments. |
| OSC Strategy Rework Discussion                | Terence introduced the strategy document. Christian reviewed the progress on previous goals (2 met, 2 pending, 1 on hold), noting need to revise goals for a potentially longer timeline. Georg Link suggested waiting until new committee members are elected before finalizing strategy goals. Jonathan agreed that the new committee makeup and approved budget are key inputs for goal setting.                                                                                                                                                                                                                                                                                                            | Defer the formal strategy rework discussion until the new committee is onboarded and the budget is finalized. Christian to potentially update the strategy status report for the onboarding process.                                                                                                                   |
| Repository Compliance & Health Metrics        | Terence presented updated data on policy compliance for 30 public repositories, noting missing or outdated governance/security policies. Christian mentioned leveraging tools (Beturgia) for health evaluation and introducing Project Baseline (OpenSSF) for security grading as a potential metric. Need to re-run the baseline assessment.                                                                                                                                                                                                                                                                                                                                                                  | Terence to continue evaluating repository compliance for the remaining repos. Christian to re-run Project Baseline assessment and discuss its use as a project metric with the Security Council.                                                                                                                       |
| New Electorate Onboarding Process             | Discussed the upcoming onboarding of new committee members/electorates. Reviewed existing onboarding slides. Potential need to update slides based on recent organizational changes. Jonathan noted the passed budget adds more concrete discussion points for onboarding. Christian suggested including mission/vision in slides.                                                                                                                                                                                                                                                                                                                                                                             | Committee members to review the onboarding document shared by Terence. Christian to update onboarding slides (add status report, mission/vision). Terence to update aged onboarding slides (e.g., service catalog). Pedro to host a separate onboarding call for new members.                                          |
| KES Project Repo Discussion                   | Jonathan reported on TSC discussion regarding KZ Agent, its potential integration into Cardano node, and whether it falls under TSC or OSC maintenance. Adam expressed dissent (via chat) citing no clear customer/user, SPO resistance, and questioning adoption/maintenance. Project aims for key security via secured memory but requires complex setup (HA, authentication). It's viewed as an incubation candidate. TSC approved, but OSC opinion sought, highlighting a case for committee dissent resolution. Ownership is IOG, developed by Well-Typed (contract potentially ending). Question raised about why Intersect (non-development org) is receiving it. Needs proper socialization with SPOs. | Committee members to consider their stance on the KZ Agent migration/incubation proposal. Jonathan/Christian to follow up with the TSC channel regarding the OSC's concerns (Adam's dissent).                                                                                                                          |
| Project Incubation Framework Discussion       | Discussion prompted by the KZ Agent case. Georg Link noted the need for clear criteria for accepting projects into an incubation program. Christian shared current categories (core, tooling, etc.) but agreed criteria need fleshing out. Georg emphasized needing defined stages, mentorship, milestones, and transition criteria.                                                                                                                                                                                                                                                                                                                                                                           | Christian to draft a proposal for project categories and criteria for the incubation process as part of the OSC vision. Georg Link to follow up offline with Christian/Terence on incorporating incubation framework references into the strategy document.                                                            |
| Onboarding Logistics & Future Chair Selection | Pedro proposed a plan for onboarding: invite leaving members to the onboarding call, host a separate call for new members, encourage remaining members to attend, and establish an 'onboarding phase' (e.g., 3 calls) before voting on a new chair. This approach allows new members to become familiar with the committee and processes before leadership decisions are made. Christian agreed with the approach.                                                                                                                                                                                                                                                                                             | Pedro to finalize and implement the proposed onboarding plan (separate call, defer chair vote).                                                                                                                                                                                                                        |
