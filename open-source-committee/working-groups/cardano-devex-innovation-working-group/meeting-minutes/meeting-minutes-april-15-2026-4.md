# Meeting Minutes - June 24, 2026

## Attendees:&#x20;

| Name                     | Attendance | Role/COI                     |
| ------------------------ | ---------- | ---------------------------- |
| Terence ‘Tex’ McCutcheon | Yes        | Lead/Secretary               |
| Bora Oben                | Yes        | Developer Advocate - CF      |
| Dan Baruka               | No         | Developer Advocate Intersect |
| Emmanuel Titi            | Yes        | Developer Advocate Intersect |
| Harun Mwangi             | Yes        | Developer Advocate Intersect |
| Uche Obasi               | No         | Developer Advocate Intersect |
| Sebastian Pabon          | No         | OSC Member                   |
| Darlisa Consoni          | No         | Ecosystem Engineering - CF   |
| Robertino Martinez       | Yes        | Product Owner - DevEx IOG    |

Community/Other Attendees

* Josefine Birkigt
* Laura Mattiucci
* Musa Ridwan Itopa



**Recording:** [Cardano Developer Experience Innovation WG - 2026/06/24 - Recording](https://drive.google.com/file/d/10gltHJgElP7Ew6NxufHACrlrg0rHNB1A/view?usp=sharing)

**Transcript:** [Cardano Developer Experience Innovation WG - 2026/06/24 - Transcript](https://docs.google.com/document/d/1izp0r1D6cZ84tZgJGw7XSOQTgzUSS64i7gYndZGT4nY/edit?usp=sharing)

## Agenda 6.24.26

* Developer Feedback Sessions
* Next steps

## Decisions/Actions

**Decisions**

* **Postpone Feedback Sessions:** Delaying the upcoming developer feedback sessions to allow ample time for proper marketing and outreach to maximize community turnout.
* **Architectural Separation of Target Audiences:** Formally separating the onboarding paths, documentation, and user journeys on the developer portal between "Application Layer/dApp Developers" and "Core/Infrastructure Developers."
* **Language Strategy for Edge Tooling:** Validated the strategic decision to build edge tooling (like the project scaffolding tools) in Rust and keep it language-agnostic to maximize external contributions, rather than forcing Haskell.
* **Developer Portal Structure:** Transitioning the portal away from fragmented categories ("get started," "learn," "build") into a centralized, 7-module sequential curriculum mapping out core workflows.
* **Strict Curation Policy:** Maintaining a strict quality gate for the Builder Tools directory to keep the portal streamlined rather than allowing it to become an uncurated catch-all repository.

**Actions**

* **Terence:** Follow up on marketing prompts and documentation in the shared folder to prepare for the rescheduled feedback session rollout.
* **Bora:** Deploy the newly restructured 7-module developer onboarding curriculum and workflow baseline to the developer portal.
* **Robertino:** Finalize the initial prototypes for the tooling integrations (working with Pebble, Pins, and Aiken) and prepare them for community review/testing within the next 1–2 months.
* **Robertino:** Conclude the current hiring process to onboard three new engineers to help scale development capacity.
* **Robertino & Bora:** Coordinate the technical integration between Robertino’s CLI scaffolding tools and the Cardano Foundation’s AI developer agent skills (created by Giovanni).
* **Laura & Marketing Committee:** Coordinate a follow-up presentation with Bora, Robertino, and Josefine in approximately 4 weeks to review the portal release baseline and launch an official promotion campaign.
* **Developer Experience Group:** Review the existing Miro board sticky notes as a "first filter" to ensure historical pain points are properly mapped against current portal deliverables before launching wider marketing.

| Topic                                             | Discussion                                                                                                                                                                                                                                                                                   | Notes                                                                                                                                                                                     |
| ------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Meeting Kickoff & Status Check                    | Bora and Robertino opened the meeting. Bora mentioned recovering from a cold despite the hot summer weather. The team decided to wait 3 minutes for additional attendees to join.                                                                                                            | Attendees caught up briefly before diving into the agenda.                                                                                                                                |
| Feedback Sessions Schedule                        | Terence raised a concern about the feedback sessions scheduled for next week. No marketing has been done yet, and with other ecosystem events happening, turnout might be low. He proposed pushing the sessions back a few weeks.                                                            | Agreed: The team agreed to delay the sessions to ensure proper marketing and better community turnout.                                                                                    |
| Marketing and Channel Strategy                    | Josefine agreed with pushing back the dates and suggested leveraging Cardano channels. She emphasized needing a clear proposition on what the sessions are for and why people should join. She noted the upcoming summer holiday season might affect July/August attendance.                 | Terence noted that the target audience (wider community seeking onboarding) might not be the ones taking traditional vacations compared to well-funded entities.                          |
| Marketing Materials & Shared Docs                 | Terence shared a new document created in the working group's shared folder containing basic marketing prompts. He requested everyone review, comment, or suggest specific adjustments to prepare for the new rollout dates.                                                                  | Document permissions were updated so all members can comment and suggest changes.                                                                                                         |
| Developer Onboarding Scope                        | Terence provided a recap of the working group's evolution from a Miro board tracking ecosystem pain points. The core strategy focuses on an open call for feedback where attendees get 1–2 minutes to share their most critical onboarding issues.                                           | The feedback targets improvements for the developer portal, developer advocate programs, and tools like Cardano Blueprint.                                                                |
| Phases of Development (Exploration vs. Execution) | Laura questioned if the group was still stuck in the early research phase rather than deploying fixes. She warned that spending too much time in exploration could delay progress for years.                                                                                                 | Terence clarified that while they are in early stages, they aim to push actionable fixes to the developer portal while actively listening to the community.                               |
| Addressing Pain Points & Filtering Issues         | Bora and Laura discussed using the original stickies on the Miro board (written by internal members/developer advocates) as a first filter. Bora suggested checking if those original issues were addressed before launching wide-scale marketing.                                           | Bora and Robertino are actively picking up and addressing portal issues one by one.                                                                                                       |
| Centralization vs. Resource Fragmentation         | Robertino highlighted that his current tooling and library work will be ready for community testing in a month. He emphasized that the biggest hurdle is incentivizing developers to contribute directly to the centralized developer portal rather than creating fragmented external sites. | The proposed strategy is to incentivize centralization by offering official ecosystem amplification (e.g., tweets/marketing) for tools added to the portal.                               |
| Curation and the Builder Tools Directory          | Bora explained that the developer portal must maintain a strict curation process to avoid becoming a "catch-all" repository. He shared a link to the updated Builder Tools directory, mirroring the approach taken with the cardano.org app store.                                           | Laura suggested having the Cardano Foundation (CF) push quarterly calls to action inviting high-quality tool submissions.                                                                 |
| Developer Portal Restructuring & Curriculum       | Bora announced he is deploying a massive restructuring of the developer portal tomorrow. The traditional "get started, learn, build" buckets are being replaced by a single, agnostic 7-module curriculum that maps out end-to-end developer workflows.                                      | This clean baseline will serve as a foundation for Robertino's upcoming proposal work.                                                                                                    |
| Haskell vs. Language-Agnostic Tooling             | Terence and Robertino debated the role of Haskell in edge tooling. Robertino defended his strategic choice to build new tooling plugins in Rust and keep them language-agnostic, noting it is incredibly difficult to recruit contributors for Haskell infrastructure.                       | Terence voiced concern that neglecting Haskell upskilling in favor of workarounds might leave the ecosystem without maintainers for its core infrastructure down the road.                |
| Differentiating Developer Profiles                | Robertino and Bora agreed that the ecosystem must separate "Application/dApp Developers" (who need fast onboarding, standard APIs, and language flexibility) from "Core/Infrastructure Developers" (who require deep Haskell knowledge to maintain ledger/consensus layers).                 | Bora emphasized that the developer portal should primarily optimize for application-layer developers to drive transaction volume.                                                         |
| Developer Advocate Program & Cohort Growth        | Terence outlined the future of the Developer Advocate program for Cohort 3, which is requesting a budget increase. The plan expands the program to six advocates: two dedicated to the DevX working group/portal, and four embedded in core technical groups.                                | The advocates will act as a bridge between outside developers and core maintainers (e.g., Ouroboros consensus).                                                                           |
| Improving Contributor-Maintainer Relations        | Robertino proposed partnering with core infrastructure teams to get them to tag "good first issues," maintain proper CI, and commit 1–2 hours a week to reviewing external pull requests. This would stop external contributions from lingering indefinitely.                                | Terence noted an ongoing adoption issue where core maintainers sometimes lack trust in the code quality of drive-by PRs or AI-generated contributions, highlighting a high bar for entry. |
| Project Tracking & Project Boards                 | Terence asked about organizing developer portal issues into a clean project board to easily track progress and present status updates to the GMC (Global Marketing Committee).                                                                                                               | Bora provided a link to the central GitHub issue he utilizes as an opinionated project board to track and interconnect smaller ecosystem contributions.                                   |
