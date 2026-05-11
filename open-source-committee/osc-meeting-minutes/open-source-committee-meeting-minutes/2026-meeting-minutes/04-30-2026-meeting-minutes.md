# (04/30/2026) Meeting Minutes

## Attendees:&#x20;

| Name                     | Attendance | Role       | Voting Seat (Y/N) | Term         |
| ------------------------ | ---------- | ---------- | ----------------- | ------------ |
| Georg Link               | No         | Chair      | Y                 | April 2026   |
| Udai Solanki             | No         | Vice Chair | Y                 | October 2026 |
| Terence ‘Tex’ McCutcheon | Yes        | Secretary  | N                 | N/A          |
| Bernard Sibanda          | No         | Member     | Y                 | October 2026 |
| Jordan Hill              | Yes        | Member     | Y                 | October 2026 |
| Philip DiSarro           | No         | Member     | Y                 | April 2026   |
| Sebastian Pabon          | Yes        | Member     | Y                 | October 2026 |
| Reshma Mohan             | Yes        | Member     | Y                 | October 2026 |
| Empty Seat               | No         | Member     | Y                 | April 2026   |
| Empty Seat               | No         | Member     | Y                 | April 2026   |
| Empty Seat               | No         | Member     | Y                 | April 2026   |

Community/Other Attendees

* Dan Baruka
* Emmanuel Titi
* Harun Mwangi
* Jean-Phillippe Raynaud
* Mike Hornan
* Samuel Leathers
* Uche Obasi



**Recording:** [Open Source Committee (Intersect) - 2026/04/30 - Recording](https://drive.google.com/file/d/1tUdEZvnGnqqRj2qsw66RmDFF71suAQ30/view?usp=sharing)

**Transcript:** [Open Source Committee (Intersect) - 2026/04/30 - Transcript](https://docs.google.com/document/d/1nikeXlZVgbGmMMwuyYY2elA7NjQJACTnNkenIDaQb-k/edit?usp=sharing)

**Chat Transcript:** [Open Source Committee Meeting – 2024/11/07 – Chat Transcript](https://drive.google.com/file/d/17SFasnZeEoVmH4j2JVgfv8dNmbDC8Avt/view?usp=sharing)

## Intros

**Tex:** Open Source Program Manager, Intersect Staff, Open Source Committee Secretary\
**Bernard:** TBD\
**Georg:** Bitergia\
**Jordan:** TBD\
**Reshma:** TBD\
**Sebastian:** OSC, Gimbalabs, contributor, Andamio co-founder.\
**Udai:** TBD

## Agenda 4.30.26

* Developer Advocate Check In
* Mithril-signer Binary
* Budget Published
* Adjustments to published Budget
* MeshAI, Midnight Setup – Tooling
* OSS Minneapolis Check In
* Security/BBP Update and Decisions
* Open Forum

## Decisions/Actions

**Decisions**

* **Approval of Mithril Signer Binary:** The committee officially "rubber-stamped" and approved the integration of the Mithril signer binary into the Cardano node artifacts.
* **Satellite Session Strategy:** It was decided that developer advocates will host local satellite events in lieu of attending the Minneapolis event in person due to visa issues.
* **Virtual Attendance Policy:** The committee decided to prioritize physical attendance for the satellite sessions to prevent crowding the meeting links; virtual participants will be accommodated via a background stream or YouTube link.
* **Security Fixes Approval:** The committee approved three low-severity security reports related to the Cardano CLI, DB Sync, and Mithril node.
* **Mesh AI/Midnight Proposal Review:** Sebastian confirmed the Mesh AI proposal is favorable for supporting onboarding, while the Midnight proposal should first seek support from the Midnight Foundation.

**Actions**

* **Terence:** Organize a coordination call in two weeks to establish rules, formats, and expectations for the Minneapolis event.
* **Terence:** Investigate if Intersect can provide financial support (rent/refreshments) for the developer advocates' satellite sessions.
* **Terence:** Set up a YouTube stream or background access for virtual attendees to watch the satellite sessions.
* **Terence:** Post official polls on Discord for the committee to formally vote on the Mesh AI and Midnight tooling proposals.
* **Mike:** Post the January through April security report in the Discord channel for committee review.
* **Mike:** Prepare a review report of all bugs processed through the tracker over the next week or two.
* **Harun, Dan, & Uche:** Meet next week to finalize their presentation for the sponsored spotlight session (including introductions and a technical demonstration).
* **Committee Members:** Review the published budget proposal on the Eleutheria platform and provide feedback or suggested adjustments in Discord.
* **Sebastian:** Lead the promotion of the budget proposal to DReps and the community to prepare for the upcoming vote.

| Topic                       | Discussion                                                                                                                                                             | Notes                                                                                                      |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| Attendance & Quorum         | Terence noted low attendance, likely due to election season. Quorum was met with half the committee present plus developer advocates.                                  | Reshma joined from vacation; Jordan, Sebastian, and Mike were also present.                                |
| Mithril Binary Integration  | Jean-Philippe (JP) proposed including the Mithril signer binary with Cardano node artifacts to improve adoption and speed up bootstrapping (30–60 mins vs. 24+ hours). | Sam confirmed this functions as a CI/CD flake input in the code, similar to the recent Daedalus release.   |
| Committee Approval          | Sebastian and Terence discussed the necessity of committee approval for maintainer program transparency and database management awareness.                             | The committee (Sebastian, Jordan, Reshma) provided a "rubber stamp" approval for the addition.             |
| Minneapolis Event Logistics | Terence provided an update on the upcoming event. Jordan, Sebastian, and Gayorg (his final event) are confirmed to attend.                                             | Uday’s attendance is pending visa confirmation. One open seat remains for a North American representative. |
| Developer Advocates Update  | Harun, Dan, and Uche were unable to obtain visas for Minneapolis. They will instead host satellite sessions and local versions of the event.                           | Terence will set up a call in two weeks to coordinate expectations and rules for the event.                |
| Satellite Sessions Support  | Harun requested financial support for renting spaces and providing refreshments for local satellite attendees.                                                         | Terence will investigate if Intersect can provide funding; individual committee support is also an option. |
| Dev Advocate Milestones     | Harun mentioned the plan to showcase running a node. The advocates will meet next week to finalize a presentation for the spotlight session.                           | Terence requested 5 minutes of introductions followed by 10-15 minutes of technical presentation.          |
| Virtual Participation       | Uche asked about sharing meeting links with virtual communities. Terence advised focusing on physical attendance to avoid crowding links.                              | Terence suggested setting up a YouTube stream for virtual observers to follow along without interrupting.  |
| Security Reports            | Mike presented three security reports for approval involving Cardano CLI, DB Sync, and the Mithril node. All are categorized as low severity.                          | The vulnerabilities related to off-chain metadata are already fixed; approval is needed for the record.    |
| Security Milestones         | Terence requested that Mike share the January–April security report and a review of the bug tracker for milestone verification.                                        | Mike agreed to share the reports in Discord for committee comments.                                        |
| Mesh AI Proposal            | Sebastian presented a proposal for Mesh AI. He argued that adding an AI layer to the widely used MeshJS library would strengthen developer onboarding.                 | Polls will be posted on Discord for a formal vote next week.                                               |
| Midnight Proposal           | Sebastian discussed a proposal regarding the Midnight ecosystem but suggested the team should seek support from the Midnight Foundation first.                         | The committee will continue the discussion in Discord before taking a final stance.                        |
| Budget Proposal             | Sebastian confirmed the budget proposal is live on the Eleutheria platform. It aligns with the work completed over previous weeks.                                     | Committee members are encouraged to review the platform version for any final adjustments.                 |
| Promotional Strategy        | The committee needs to begin active promotion of the budget to delegates (DReps) and the wider community to ensure successful voting.                                  | Sebastian noted that the final PDF and platform versions appear to be in sync.                             |
