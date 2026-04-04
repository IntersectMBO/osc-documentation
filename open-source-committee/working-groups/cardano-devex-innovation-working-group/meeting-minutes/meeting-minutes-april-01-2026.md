# Meeting Minutes - April 01, 2026

## Attendees:&#x20;

| Name                     | Attendance | Role/COI                     |
| ------------------------ | ---------- | ---------------------------- |
| Georg Link               | No         | OSC Chair                    |
| Terence ‘Tex’ McCutcheon | Yes        | Lead/Secretary               |
| Kyle Solomon             | Yes        | CPC Vice Chair               |
| Bora Oben                | Yes        | Developer Advocate - CF      |
| Dan Baruka               | No         | Developer Advocate Intersect |
| Emmanuel Titi            | Yes        | Developer Advocate Intersect |
| Harun Mwangi             | Yes        | Developer Advocate Intersect |
| Uche Obasi               | No         | Developer Advocate Intersect |
| Sebastian Pabon          | Yes        | OSC Member                   |
| Darlisa Consoni          | Yes        | Ecosystem Engineering - CF   |
| Robertino Martinez       | Yes        | Product Owner - DevEx IOG    |

Community/Other Attendees

* Bernard Sibanda



**Recording:** [Cardano Developer Experience Innovation WG - 2026/04/01 - Recording](https://drive.google.com/file/d/11goFuGNU_vR9R2MVisjHfNCNIyO5BOh5/view?usp=sharing)

**Transcript:** [Cardano Developer Experience Innovation WG - 2026/04/01 - Transcript](https://docs.google.com/document/d/1xOnTCpRVj4GyBUsoxboRTvwM4mEcudHgE0R9EFK9Nrk/edit?usp=sharing)

**Chat Transcript:** [DevEx Innovation WG Meeting – 2026/04/01 – Chat Transcript](https://drive.google.com/file/d/10XWW0blqSCCZdvVGZIdRwjZ-X33N3jGw/view?usp=sharing)

## Agenda 4.01.26

* Continuation of Developer Onboarding

## Decisions/Actions

**Decisions**

* **Documentation Focus:** The group decided that high-level documentation should be consolidated on the Developer Portal, while repository-specific documentation remains on individual sites.
* **SPO Track Exclusion:** There is an agreement to exclude Stake Pool Operator (SPO) tracks from the detailed contributor journey for now, as sufficient documentation already exists for that path.
* **Primary Development Language:** The "North Star" for new training and curricula will be Aiken rather than Plutus/Haskell, to reflect current developer preferences and ease of onboarding.
* **Strategy Duration:** Robertino decided to shorten the initial funding proposal to a 6-month sprint (to be completed by November 2026) to validate ideas before committing to a full 12-month cycle.
* **Windows Support:** Robertino committed to prioritizing Windows as a primary OS for his "get started" tooling to address the friction faced by developers in Africa and Asia.
* **Meeting Cadence:** The weekly meeting schedule will transition to a monthly 90-minute session starting in May or June 2026.

Actions

* **Terence:** Follow up with the Developer Advocates to confirm if a new branch or PR has been created on the Dev Portal repo for the contributor flow.
* **Terence:** Coordinate with the Open Source Committee (OSC) and Product Committee to get a unified endorsement for new DevX proposals.
* **Robertino:** Update the Plutus Pioneer Program (PPP) repository with a prominent warning label stating that the content is outdated and providing links to newer resources.
* **Bora & Robertino:** Connect outside of the working group to collaborate on the "Zero to Hero" curriculum, merging Robertino’s Spanish resources with Bora’s ongoing work.
* **All Members:** Review Robertino’s DevX strategy/roadmap and "sign off" by acknowledging the repo or opening issues for any points of disagreement.
* **Kyle & Robertino:** Assess whether a small contract can be kicked off to a community developer to help revamp or modernize specific training modules.
* **Bernard:** Continue providing feedback on the specific "pain points" of university students to ensure the new tools remain accessible to non-functional/Windows-based programmers.

| Topic                                     | Discussion                                                                                                                                                                                                             | Notes                                                                                                                                       |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| BuidlerFest & Hackathon Recap             | Robertino shared experiences from the recent BuidlerFest. 20 teams participated in the hackathon; about half were new to Cardano. Robertino provided architectural guidance and confirmed successful Pyth integration. | Winners are decided; PRs likely to remain as-is rather than being merged into the SDK due to the nature of the submissions.                 |
| Documentation Hierarchy                   | Terence raised the need for a "middle ground" in documentation. Currently, there are high-level docs on the Dev Portal and repo-specific docs, but the space between needs better tracking.                            | Discussion on creating a documentation map to clarify the hierarchy between portal and repo levels needed.                                  |
| Contributor Journey & Portal Updates      | The group checked the status of the detailed contributor journey branch on the Dev Portal repo. Bora confirmed no open PR or active branch is visible yet.                                                             | Action: Terence to follow up with the team to ensure the branch for the contributor flow is established.                                    |
| Tooling Strategy: "Can I Use" for Cardano | Robertino proposed a feature similar to "Can I Use" for web standards, mapping Cardano standards across various off-chain libraries to help developers choose tools.                                                   | Bora agreed this is possible and aligns with providing "tooling bundles" for specific use cases (e.g., DApp backends).                      |
| IOG DevX Roadmap Alignment                | Sebastian and Bora discussed aligning the working group’s efforts with the IOG DevX repository roadmap. Bora highlighted the plan as solid and holistic.                                                               | Members are encouraged to review the roadmap and sign off or open issues to ensure collaborative alignment.                                 |
| Education: Zero-to-Production Curriculum  | Bora is developing a comprehensive curriculum targeting universities and professional education, focusing on taking developers from zero to "hackathon-ready."                                                         | The curriculum will focus on modern tools (Aiken, Mesh) and practical, project-based learning.                                              |
| Plutus Pioneer Program (PPP) Status       | The group debated the current validity of the PPP. Robertino noted it is roughly 70% useful but uses deprecated tools like Lucid and older Aiken versions.                                                             | General consensus: PPP should not be the primary entry point for new devs as outdated code causes frustration.                              |
| Revamping Smart Contract Training         | Bernard emphasized the heavy use of PPP in university settings despite its age. Robertino suggested a "strip down" approach focusing on isolated scripts rather than full front-end integration.                       | Action: Explore a collaborative workstream to modernize the curriculum, potentially as a "Cardano Application Development" flagship course. |
| Developer Onboarding Barriers             | Bernard noted that 90% of struggling devs are used to imperative programming and Windows OS. Transitioning to functional paradigms and Linux/Docker environments is a major hurdle.                                    | Robertino committed to targeting Windows as a primary OS for upcoming "get started" tooling to lower the entry barrier.                     |
| Language & Global Reach                   | Discussion on the importance of translations. Robertino has content in Spanish, and Bernard has translated materials into French and is targeting Asian languages.                                                     | Future resources should be designed for easy translation to support the global community (Africa, Asia, etc.).                              |
| Aiken vs. Plutus                          | Bora and Robertino agreed that modern core development has shifted toward Aiken. Reference materials may remain in Plutus/Haskell, but the "North Star" path should be Aiken-based.                                    | Training must be data-driven, focusing on what developers are actually using to build production apps.                                      |
| KPIs & Developer Metrics                  | Bora argued that the primary KPI should be increasing the unique developer activity count to improve Cardano's standing in industry reports (e.g., Electric Capital).                                                  | Goal: Create a "speedrun" experience where a developer can get a test passing in under a minute.                                            |
| Funding & Strategy Timeline               | Robertino is adjusting the DevX strategy proposal to a 6-month sprint for the treasury to validate ideas, while maintaining a 12-month overarching vision.                                                             | Terence suggested presenting the proposal to the Open Source Committee (OSC) and Product Committee for unified endorsement.                 |
| Meeting Cadence Change                    | Terence announced that the weekly cadence will soon move to a monthly 90-minute session (last Wednesday of every month) starting in May/June.                                                                          | Final weekly meetings will conclude over the next couple of weeks.                                                                          |
