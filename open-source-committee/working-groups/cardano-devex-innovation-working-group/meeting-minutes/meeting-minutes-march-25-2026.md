# Meeting Minutes - March 25, 2026

## Attendees:&#x20;

| Name                     | Attendance | Role/COI                     |
| ------------------------ | ---------- | ---------------------------- |
| Georg Link               | No         | OSC Chair                    |
| Terence ‘Tex’ McCutcheon | Yes        | Lead/Secretary               |
| Kyle Solomon             | Yes        | CPC Vice Chair               |
| Bora Oben                | No         | Developer Advocate - CF      |
| Dan Baruka               | Yes        | Developer Advocate Intersect |
| Emmanuel Titi            | Yes        | Developer Advocate Intersect |
| Harun Mwangi             | Yes        | Developer Advocate Intersect |
| Uche Obasi               | No         | Developer Advocate Intersect |
| Sebastian Pabon          | Yes        | OSC Member                   |
| Darlisa Consoni          | Yes        | Ecosystem Engineering - CF   |
| Robertino Martinez       | No         | Product Owner - DevEx IOG    |

Community/Other Attendees

* Josefine Birkigt
* P. Lucas
* Samuel Leathers
* Tommy Kammerer



**Recording:** [Cardano Developer Experience Innovation WG - 2026/03/25 - Recording](https://drive.google.com/file/d/1RzXhdvXy5WpAjGbTBuGYLstYowGDIGCa/view?usp=sharing)

**Transcript:** [Cardano Developer Experience Innovation WG - 2026/03/25 - Transcript](https://docs.google.com/document/d/1NMBqdpoEgnf6UM7Qwd9OeHVEWbSp1aM8ZVFMaH7AphI/edit?usp=sharing)

**Chat Transcript:** [DevEx Innovation WG Meeting – 2026/03/25 – Chat Transcript](https://drive.google.com/file/d/1RhbMSjnb8LKVGaG2mtzpWWQdWtgs5abi/view?usp=sharing)

## Agenda 3.25.26

* Developer Journey: From Zero to Core Contributor (Dan B.)

## Decisions/Actions

**Decisions**

* **Documentation Hierarchy:** High-level documentation will remain on the Developer Portal, while repository-specific details will stay in the individual repo sites.
* **Target Audience Scope:** The working group will exclude Stake Pool Operator (SPO) tracks from this specific developer pathway to maintain focus, noting that exhaustive SPO documentation already exists.
* **Tooling Strategy:** Rather than creating a new, separate list of developer tools, the group decided to integrate the existing JavaScript-maintained list of \~100 tools into the pathway.
* **Technical Framework:** The pathway will be maintained using Mermaid Markdown to allow for easy collaboration and AI-assisted gap analysis.
* **CLARIFICATION - Publishing Cadence:** The Developer Portal will follow a standard Friday push from staging to main, requiring three approvals for any PR.

**Actions**

* **\[Dan & Tommy]** Audit and update all links in the diagram to ensure they are current and functional before submitting a PR to the official Developer Portal.
* **\[Samuel]** Use an AI agent (Hayate) to test the "Indexer" workflow and identify specific technical gaps or "black holes" in the current documentation.
* **\[Tommy]** Provide GitHub write permissions for the Developer Portal to Dan (and others as requested) to facilitate reviews and staging updates.
* **\[All]** Review the pathway specifically to identify and remove legacy or unmaintained content (e.g., outdated Plutus Pioneer materials or Marlowe references).
* **\[Terence]** Add Josefine to the recurring meeting invite list for future sessions.

| Topic                       | Discussion                                                                                                                           | Notes                                                                                                                                     |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------- |
| 1. Welcome & Updates        | Terence and Tommy opened the meeting. Darlisa requested updates from the previous week's session which she missed.                   | Terence mentioned that minutes from last week are available and covered the developer onboarding breakdown.                               |
| 2. Documentation Levels     | Discussion on the distinction between high-level documentation (Developer Portal) and low-level documentation (repository-specific). | High-level docs help developers decide to join; repo docs provide technical build steps. Agreement needed on maintaining synchronization. |
| 3. Developer Pathway Reveal | Dan presented a draft of a "Developer Pathway" diagram designed to guide users from "Zero to Core Contributor."                      | The path includes categories for Beginners, Web2 Developers, and UI/UX Designers.                                                         |
| 4. Cardano Fundamentals     | Dan highlighted that all entrants must learn EUTXO models, native tokens, and Ouroboros regardless of their starting point.          | Suggested resources: Cardano Academy, Gimbalabs, and official Cardano courses.                                                            |
| 5. Specialized Tracks       | The diagram branches into Smart Contracts, Front-end/DApps, Infrastructure, and "Non-code/Finance" roles.                            | Smart contract options include Aiken and Plutus V3; Front-end focuses on SDKs like Mesh, Lucid, or Blaze.                                 |
| 6. Ecosystem Onramps        | Darlisa inquired about specific paths for developers coming from other ecosystems like Ethereum or Solana.                           | Dan noted they must learn the UTXO model specifically but can likely skip general blockchain basics.                                      |
| 7. Legacy Tooling Audit     | Kyle and Samuel raised concerns about including outdated or unmaintained programs like "Plutus Pioneers" and "Marlowe."              | Decision: Audit all links and remove "legacy" content to avoid confusing new developers.                                                  |
| 8. Tooling Gaps             | Samuel pointed out "black holes" in the workflow, specifically regarding testing tools and low-resource indexer development.         | The group will use these gaps to identify where new documentation or resources need to be prioritized.                                    |
| 9. Stake Pool Operators     | The group discussed whether to include Stake Pool Operator (SPO) paths in this specific developer guide.                             | Consensus: Exclude SPO tracks for now as exhaustive documentation already exists elsewhere.                                               |
| 10. Implementation Format   | The pathway is currently built using Mermaid (markdown) to allow for easy text-based editing and AI analysis.                        | Tommy suggested integrating the existing list of \~100 developer tools rather than creating a new, separate list.                         |
| 11. Migration to Dev Portal | The goal is to move this pathway from the working group's repo to the official Developer Portal.                                     | Samuel suggested working on a branch until the content is more polished.                                                                  |
| 12. Open Source Summit      | Terence discussed a sponsorship/booth at an upcoming summit in Minneapolis (May 18-20).                                              | Kyle and Adam may coordinate an "activation" (e.g., Hydra events) to draw traffic to the Cardano booth.                                   |
| 13. New Attendee Intro      | Josefine introduced herself, stating she is joining to listen and align her work with the group's progress.                          | Terence will add her to the recurring invite list.                                                                                        |
| 14. PR Process              | Tommy explained the "Staging to Main" workflow: PRs require three approvals and are pushed to production on Fridays.                 | Contributors are encouraged to work on personal forks of the Docusaurus-based site.                                                       |
