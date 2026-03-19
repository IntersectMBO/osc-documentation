# Meeting Minutes - March 18, 2026

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
| Darlisa Consoni          | No         | Ecosystem Engineering - CF   |
| Robertino Martinez       | Yes        | Product Owner - DevEx IOG    |

Community/Other Attendees

* Bevan Mauya
* Musa Ridwan Itopa
* Samuel Leathers
* Tommy Kammerer



**Recording:** [Cardano Developer Experience Innovation WG - 2026/03/18 - Recording](https://drive.google.com/file/d/10mLxzGZc2zwDShTO1cgvqmlv5JiJlF-Z/view?usp=drive_link)

**Transcript:** [Cardano Developer Experience Innovation WG - 2026/03/18 - Transcript](https://docs.google.com/document/d/1cg-gk0huIowT_nOclzxSFJ6OufIQ-nFyRbeseOhu5a8/edit?usp=sharing)

**Chat Transcript:** [DevEx Innovation WG Meeting – 2026/03/18 – Chat Transcript](https://drive.google.com/file/d/1rMUQ1XIm6iF3eK7UD02vQlu5-7AEBNIY/view?usp=sharing)

## Agenda 3.18.26

* Developer Onboarding Breakdown

## Decisions/Actions

**Decisions**

* **Focus on Developer Portal:** A general consensus was reached to prioritize work and resources on developers.cardano.org to combat resource fragmentation.
* **Target Audience Definition:** The group agreed that the primary target audience for current onboarding efforts is developers who are new to Cardano but want to build functional DApps.
* **Onboarding Baseline:** Defined the onboarding "success" point as a developer being able to understand the UTXO model, write/sign a contract, serialize it, and connect it to a frontend.
* **Documentation Philosophy:** Agreed that high-level "how-to" documentation should be centralized (likely on the developer portal), while low-level technical documentation (like Haddock) should remain close to the code repositories and be auto-updated.
* **Bifurcated Funnels:** Acknowledged the need for two distinct paths: one for Core Tech contributors (maintaining the node/ledger) and one for DApp developers (using high-level tools like Mesh or Aiken).

**Actions**

* **Resource Mapping (Terence):** Start an issue thread or discussion on the developer portal to begin collecting and cataloging all existing high-level documentation resources.
* **Bora’s Documentation (Bora/Tommy):** Document the specific decisions and current state of progress made in previous sessions (Tommy filling in for Bora).
* **Repo Issues (Robertino/Everyone):** Create a series of issues in Oven’s repository to translate the current Miro board brainstorms into actionable tasks.
* **Educational Asset Review (Terence):** Continue testing and exploring how to host the former Emergo Academy source files, potentially using the Andamio platform.
* **Internal Consolidation Talk (Robertino):** Speak internally at IO to see if specific core tech documentation can be transferred or consolidated under Intersect to reduce "subdomain bloat."
* **Agenda for Next Week (Group):** Map out the known resources collected from the new issue thread to identify exactly what needs to be "corralled" and consolidated.

| Topic                     | Discussion                                                                                                                                                                       | Notes                                                                            |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| Project Focus             | Terence summarized the consensus from previous weeks: the primary focus is now on developers.cardano.org to address resource fragmentation.                                      | Strategy is shifting toward centralized documentation.                           |
| Developer Onboarding      | The group discussed what "onboarding" actually means. Robertino defined the baseline as a developer being able to build a simple DApp (contracts, transactions, and frontend).   | Agreement that onboarding depends on the developer's background (Web2 vs. Web3). |
| Infrastructure Barriers   | Robertino argued that managing a Cardano node isn't strictly necessary for onboarding, as devs can use intermediate interfaces like Blockfrost.                                  | Goal is to lower the barrier to entry for initial building.                      |
| Marketing & Retention     | Kyle suggested using retargeting tags on documentation. If a developer visits and leaves, marketing spend can trigger ads to bring them back into the funnel.                    | Aim is to treat the developer portal as a conversion funnel.                     |
| Advocate Experience       | Harun and Dan shared insights from the last six months. A major hurdle is the "path to opportunity"—showing devs how to go from learning to earning/contributing.                | Fragmented and outdated docs remain a significant blocker.                       |
| "Five-Minute" Success     | Sebastian emphasized the need for a "5-minute build" experience. Developers need immediate "hits of happiness" to stay engaged with the complex Cardano stack.                   | Immediate feedback loops are key to retention.                                   |
| Hello World Tutorials     | Kyle and Dan proposed creating 3-5 distinct "Hello World" paths (e.g., submitting a transaction vs. minting an asset) to cater to different developer interests.                 | Provide multiple entry points to the ecosystem.                                  |
| Smart Contract Simulation | Samuel noted a major ecosystem failure: the lack of an easy environment to simulate smart contracts without a full node or advanced Haskell knowledge.                           | Need for a "Plutus Development Platform" or sandbox.                             |
| Intersect's Scope         | Terence clarified that Intersect (via Developer Advocates) acts as a steward for core repositories. Funding for new tooling may come through the Tooling Sustainability Program. | Distinction made between documentation work and tool development.                |
| Educational Resources     | Harun mentioned the now-closed Emergo Academy. Terence confirmed he has the source files and is exploring hosting them via the Andamio platform for Intersect members.           | Potential for a token-based "certificate of completion" for learners.            |
| Core vs. DApp Funnels     | Robertino suggested splitting onboarding into two paths: one for Core Tech contributors (node, ledger) and one for DApp developers (Mesh, Aiken).                                | Profiles and skill sets for these two groups are vastly different.               |
| Documentation Hierarchy   | The group discussed a three-tier doc structure: Beginner (high-level), Intermediate (how-to guides), and Top-level (auto-generated API/Haddock docs).                            | High-level docs should be centralized; low-level docs stay near the code.        |
| Consolidation Strategy    | Robertino proposed consolidating various IO and Intersect subdomains into a single "Core Tech" documentation cluster to reduce confusion.                                        | Goal: A "single source of truth" for core contributors.                          |
| Action Items              | Terence suggested starting an issue thread/discussion on the developer portal to collect and map all existing high-level resources.                                              | The next meeting will focus on mapping these resources.                          |
