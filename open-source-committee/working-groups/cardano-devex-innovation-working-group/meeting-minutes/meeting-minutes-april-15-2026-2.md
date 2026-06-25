# Meeting Minutes - April 29, 2026

## Attendees:&#x20;

| Name                     | Attendance | Role/COI                     |
| ------------------------ | ---------- | ---------------------------- |
| Terence ‘Tex’ McCutcheon | Yes        | Lead/Secretary               |
| Bora Oben                | Yes        | Developer Advocate - CF      |
| Dan Baruka               | Yes        | Developer Advocate Intersect |
| Emmanuel Titi            | Yes        | Developer Advocate Intersect |
| Harun Mwangi             | Yes        | Developer Advocate Intersect |
| Uche Obasi               | No         | Developer Advocate Intersect |
| Sebastian Pabon          | Yes        | OSC Member                   |
| Darlisa Consoni          | Yes        | Ecosystem Engineering - CF   |
| Robertino Martinez       | Yes        | Product Owner - DevEx IOG    |

Community/Other Attendees

* Bernard Sibanda
* Josefine Birkigt
* Seun Gibri



**Recording:** [Cardano Developer Experience Innovation WG - 2026/04/29 07:00 CDT - Recording](https://drive.google.com/file/d/1uM_BL6dyqrTQnw795qjSgo13Ywl5BRmi/view?usp=sharing)

**Transcript:** [Cardano Developer Experience Innovation WG - 2026/04/29 07:00 CDT - Transcript](https://docs.google.com/document/d/1bdUhBw1jPXwthGQ9rl47hr7U9YdXigo3Hlly1nS1VkU/edit?usp=sharing)

## Agenda 4.29.26

* Developer Experience Innovation updates

## Decisions/Actions

**Decisions**

* **Next Meeting Format:** The team decided to format next month's meeting as a fully broadcasted, open live feedback session rather than a standard closed meeting.
* **Open Session Rules:** It was decided to limit individual speaking time during the open session to 60 seconds (or 1–2 minutes maximum) per developer to quickly capture their biggest friction points.
* **Document Overhaul Strategy:** The group agreed that the immediate mandate for Developer Advocates regarding documentation is to use minor error fixes as an onboarding pipeline for new contributors, rather than attempting a massive standalone documentation rewrite.
* **Communication Channel Consolidation:** The team decided to streamline support pathways by directing all community technical friction points to two specific channels: the Intersect DevX Discord and the Cardano Foundation (CF) Engineering Discord.

**Actions**

* **Terence & Bora:** Coordinate in the background over the next few days to figure out the logistical setup, marketing, and multiplatform streaming options for the upcoming open feedback session.
* **Bora:** Follow up internally with his team and review/approve Dan's open Pull Request (PR) for the interactive map on the Developer Portal.
* **Bora:** Catch up with Robertino regarding the timeline and community transition plan for the "Cardano Init" tool proposal, as well as steering the $3M DevX proposal to prevent ecosystem silos.
* **Bernard:** Encourage his Coxygen students and any struggling beginners to actively use the newly streamlined Discord channels and attend the Friday developer office hours.

| Topic                                          | Discussion                                                                                                                                                                                                                                               | Notes                                                                                                                     |
| ---------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| 1. Meeting Kick-off & Expectations             | Terence opened the call, waiting a few minutes for attendees to join before pivoting the focus onto the main developer experience agenda and future timelines.                                                                                           | Next meeting is tentatively scheduled in roughly four weeks (one month).                                                  |
| 2. Event Booth Location Strategy               | Terence and Bora discussed optimization for the upcoming event booth. Bora shared insights from a previous Java conference, highlighting that corner locations and spots near mixed-use spaces or workshop entrances/exits yield the highest visibility. | Positions near the "Sponsor Recharge" (coffee/water area) or layout spots like G6/12 were favored over closed spaces.     |
| 3. Governance & Budget Proposals               | Terence noted a recent wave of governance actions touching on developer experience. He highlighted that their specific budget proposal—which funds the Developer Advocate program and the Paid Open Source Model (POSM)—is nearing completion.           | The group aims to align internal work streams with external ecosystem proposals to ensure efficiency.                     |
| 4. Documentation as a Contribution Entry Point | Terence clarified that tasks assigned to Developer Advocates regarding documentation are meant to serve as low-friction entry points for new contributors to engage with the core codebase, rather than a standalone documentation overhaul.             | Finding an error and submitting a PR is viewed as a qualitative first step to engage with core maintainers.               |
| 5. AI Usage in Documentation                   | Bora and Terence debated AI-generated documentation. Bora mentioned utilizing AI to test native readiness and identify gaps, but Terence recalled historical negative community feedback regarding fully AI-drafted content.                             | The consensus is that experienced human developers need to drive documentation quality to avoid "AI crap" complaints.     |
| 6. Cardano Init Tool Integration               | Dan, Terence, and Bora discussed the "Cardano Init" tool (a bootstrapping CLI tool from the IO treasury proposal). The team discussed whether it belongs in the Intersect repository or alongside the Developer Portal.                                  | The tool is a 6-month program intended to transition to community/POSM maintenance post-launch.                           |
| 7. Developer Portal Updates                    | Bora provided an update on the Developer Portal, noting it focuses heavily on the application layer. Dan submitted a PR for an interactive map, which received minor feedback to align with default Docusaurus components and is ready to merge.         | Bora is also working on adding extensive content to improve AI agent readiness on the portal.                             |
| 8. Measuring Community Impact                  | Terence questioned how to accurately measure if the team has successfully influenced a better DevX over the past two months. Bora noted that traditional written surveys yield low-quality engagement.                                                   | The team agreed that written feedback methods are often too idealistic for broader developer audiences.                   |
| 9. Open Live Feedback Session Initiative       | Sasha, Terence, and Bora brainstormed hosting next month's meeting as a fully broadcasted, open-hour live session. Developers will get 60–90 seconds to state their biggest friction points on mic.                                                      | Bora suggested streaming across multiplatform channels (e.g., the main Cardano account) to maximize reach.                |
| 10. Core Tech Contribution & Mentorship        | Bora asked how Developer Advocates interact with core repo maintainers. Emmanuel explained their current flow: Advocates act as the "glue," pairing interested community developers with repository maintainers to expedite PR reviews.                  | Developer Advocates aim to onboard a minimum of 8 new developers per quarter (2 per advocate) to core repositories.       |
| 11. Coxygen Project & Ecosystem Friction       | Bernard shared his experience running Coxygen (funded via Catalyst to onboard students to Plutus). He reported that while the Developer Portal has improved significantly, onboarding beginners remains far more challenging than in Ethereum or Solana. | Bernard emphasized the critical need for a sandbox/playground tool (similar to Solana Playground) for complete beginners. |
| 12. Mitigating Ecosystem Silos                 | Bora and Bernard discussed a $3M IO proposal for DevX, stressing that funded ecosystem projects must be steered by or aligned with this working group to avoid creating disjointed, short-lived functional silos.                                        | Bora communicated this intent to Robertino to ensure the working group remains a core steering unit.                      |
| 13. Streamlining Social Channels               | Bora urged members to direct students and developers facing friction to active channels like the Intersect DevX Discord or the Cardano Foundation Engineering Discord.                                                                                   | Low traction on social channels makes it difficult for maintainers to diagnose hidden friction points.                    |
| 14. Wrap-up & Action Items                     | Terence concluded the meeting, thanking participants and laying out immediate next steps regarding notes dissemination and background coordination.                                                                                                      | Terence to distribute official minutes within 1–2 days and coordinate the upcoming open session logistics with Bora.      |
