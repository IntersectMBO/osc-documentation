---
hidden: true
---

# (04/16/2026) Meeting Minutes

## Attendees:&#x20;

| Name                     | Attendance | Role       | Voting Seat (Y/N) | Term         |
| ------------------------ | ---------- | ---------- | ----------------- | ------------ |
| Georg Link               | Yes        | Chair      | Y                 | April 2026   |
| Udai Solanki             | No         | Vice Chair | Y                 | October 2026 |
| Terence ‘Tex’ McCutcheon | Yes        | Secretary  | N                 | N/A          |
| Bernard Sibanda          | No         | Member     | Y                 | October 2026 |
| Jordan Hill              | Yes        | Member     | Y                 | October 2026 |
| Sebastian Pabon          | Yes        | Member     | Y                 | October 2026 |
| Reshma Mohan             | Yes        | Member     | Y                 | October 2026 |
| Empty Seat               | No         | Member     | Y                 | April 2026   |
| Empty Seat               | No         | Member     | Y                 | April 2026   |
| Empty Seat               | No         | Member     | Y                 | April 2026   |
| Empty Seat               | No         | Member     | Y                 | April 2026   |

Community/Other Attendees

* Benjamin Hart
* Dan Baruka
* Emmanuel Titi
* Harun Mwangi
* Luke Mahoney
* Newman Lanier



**Recording:** [Open Source Committee (Intersect) - 2026/04/16 - Recording](https://drive.google.com/file/d/1D2WE_thSeSZ-MK28ou49Wh1UEFYVxD7V/view?usp=sharing)

**Transcript:** [Open Source Committee (Intersect) - 2026/04/16 - Transcript](https://docs.google.com/document/d/1ErovfT0WCRlWm0j0ZLBkLQT4aXUMt84WmHYD7UuQzoU/edit?usp=sharing)

**Chat Transcript:** [Open Source Committee Meeting – 2024/11/07 – Chat Transcript](https://drive.google.com/file/d/14XbqdwZiamjGby2w4dNZTr4FzzqMXnz-/view?usp=sharing)

## Intros

**Tex:** Open Source Program Manager, Intersect Staff, Open Source Committee Secretary\
**Bernard:** TBD\
**Georg:** Bitergia\
**Jordan:** TBD\
**Reshma:** TBD\
**Sebastian:** OSC, Gimbalabs, contributor, Andamio co-founder.\
**Udai:** TBD&#x20;

## Agenda 4.16.26

* Developer Advocate Check-In
* MLabs - Tooling Projects
* Confirmation of 2026 Budget
* MRP Task Expectations
* MRP Interview Calendar?
* Accelerator/PSS Metadata

## Decisions/Actions

**Decisions**

* **Voting Method:** The committee decided to conduct formal voting on the MLabs tooling projects via Discord polls rather than during the meeting due to a lack of quorum.
* **Poll Structure:** Polls will run for seven days with a simple "Yes/No" format (no "Abstain" option).
* **Budget Framework:** The overall framework and funding amounts for the new budget proposal were finalized, leaving only minor polishing.
* **Maintainer Reporting:** Agreed on a middle-ground reporting approach where maintainers provide a markdown-based report of tasks, supplemented by automated dashboard data to reduce overhead.

**Actions**

* **MLabs (Benjamin/Luke):** Draft a detailed document outlining requested funding amounts and milestones for the maintenance of their tools using the standard Intersect template.
* **Terence:** Update the original tooling applications with the new information provided by MLabs and link them for committee review in Discord.
* **Terence:** Post five separate polls on Discord for the committee to vote on the MLabs projects (CTL, Covenant, YTXP Lib, TX Village, and Lambda Buffers).
* **Committee Members:** Review the Q1 Benefit Report and Q1 Progress Report to provide approval for milestone payments.
* **Committee Members:** Provide "time blocks" for upcoming maintainer interviews over the next six weeks.
* **Georg & Terence:** Perform a final review and "touch-up" of the budget proposal over the weekend for submission early next week.
* **Sebastian:** Review the maintainer task file (CSV/Template) to ensure compatibility with the back-end system for loading tasks.

| Topic                             | Discussion                                                                                                                                        | Notes                                                                                                                 |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| Call to Order & Quorum            | Georg opened the meeting. Quorum was not met; therefore, no formal votes could be resolved during the call.                                       | Meeting to be recorded for absent members; ClickUp used for the agenda.                                               |
| Developer Advocate Update         | Emmanuel discussed the start of Q2 plans, focusing on "post-build" insights for community members.                                                | Focus is on helping builders move from product completion to target audience communication.                           |
| MLabs Tooling: CTL & Plutonomicon | Luke and Benjamin presented Cardano Transaction Lib (CTL) as a highly open-source tool with significant external adoption (Indigo, Liqwid).       | Seeking funding to introduce JavaScript bindings to move away from the PureScript limitation.                         |
| Funding & Maintainership          | Georg questioned the open-source practices of MLabs. Benjamin and Luke noted that while MLabs are main maintainers, they seek broader engagement. | The committee is looking for healthy "README" and "CONTRIBUTING" files and active issue trackers.                     |
| Tooling Maintenance Roadmap       | Terence asked for a roadmap aligned with hard forks and upgrades. Benjamin confirmed the focus is on bug fixes and compatibility.                 | MLabs tasked to draft specific funding amounts and milestones using the standard Intersect template.                  |
| Covenant Project                  | Benjamin described Covenant as "LLVM for Plutus," acting as a compilation middleware for language developers (e.g., used by Konma).               | Highlighted organic adoption by external companies as evidence of tool utility.                                       |
| YTXP Lib & TX Village             | Benjamin explained YTXP Lib for upgradeable smart contracts and TX Village as a Rust pipeline for simplified transaction building.                | Georg noted these have less visible external engagement compared to CTL.                                              |
| Lambda Buffers                    | A tool for type sharing across Haskell, Rust, and JavaScript using a protocol buffer-style binary format.                                         | Developed via Catalyst; intended to improve dev-experience across multi-language stacks.                              |
| Budget Proposal                   | Georg and Terence discussed the new budget for tooling sustainability, developer advocates, and metrics.                                          | Final review/touch-ups due over the weekend; submission expected early next week.                                     |
| Maintainer Retainer Program       | Terence presented a draft template for maintainer tasks to ensure accountability and active engagement.                                           | Georg suggested aligning language across months (e.g., month 2 vs. month 5) to ensure consistent triage expectations. |
| Program Deadlines                 | Terence noted a \~60-day window (ending approx. June 20-24) to onboard maintainers under the current fee structure.                               | Maintainers must have signed contracts by the late June cutoff.                                                       |
| Reporting & Dashboards            | Discussion on using a data dashboard to track response times, reducing the manual reporting burden on maintainers.                                | Goal is to grade maintainers on explicit reporting while verifying via automated metrics where possible.              |
| Quarterly Benefit Reports         | Terence presented the Q1 Benefit Report and Q1 Progress Report for committee review.                                                              | Milestone-dependent reports required to release funds for travel and developer advocate payments.                     |
| Discord Voting                    | Terence announced that five separate polls (one per tool) will be posted on Discord for formal committee voting.                                  | Polls will run for 7 days with "Yes/No" options; no "Abstain" option included per agreement.                          |
