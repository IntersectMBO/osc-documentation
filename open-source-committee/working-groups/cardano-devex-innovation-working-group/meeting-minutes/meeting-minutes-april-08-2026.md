# Meeting Minutes - April 08, 2026

## Attendees:&#x20;

| Name                     | Attendance | Role/COI                     |
| ------------------------ | ---------- | ---------------------------- |
| Georg Link               | No         | OSC Chair                    |
| Terence ‘Tex’ McCutcheon | Yes        | Lead/Secretary               |
| Kyle Solomon             | No         | CPC Vice Chair               |
| Bora Oben                | Yes        | Developer Advocate - CF      |
| Dan Baruka               | Yes        | Developer Advocate Intersect |
| Emmanuel Titi            | Yes        | Developer Advocate Intersect |
| Harun Mwangi             | Yes        | Developer Advocate Intersect |
| Uche Obasi               | No         | Developer Advocate Intersect |
| Sebastian Pabon          | Yes        | OSC Member                   |
| Darlisa Consoni          | No         | Ecosystem Engineering - CF   |
| Robertino Martinez       | Yes        | Product Owner - DevEx IOG    |

Community/Other Attendees

* Bernard Sibanda
* Josefine Birkigt



**Recording:** [Cardano Developer Experience Innovation WG - 2026/04/08 - Recording](https://drive.google.com/file/d/1wVI4zLiujWvhRVXC-roqGymNZLKc93CU/view?usp=sharing)

**Transcript:** [Cardano Developer Experience Innovation WG - 2026/04/08 - Transcript](https://docs.google.com/document/d/1fLfAAd7lgmcFmLS3iHEJlIsmGaFuedcdtp2-kAyZuXQ/edit?usp=sharing)

**Chat Transcript:** [DevEx Innovation WG Meeting – 2026/04/08 – Chat Transcript](https://drive.google.com/file/d/1Hix_hbNl4TJc6ZxVeGOOYcBVePeNrFnS/view?usp=sharing)

## Agenda 4.08.26

* Continued Discussion

## Decisions/Actions

**Decisions**

* **Standardized Tech Stack for Onboarding:** The group reached a consensus to use an opinionated, "standard" tech stack for the initial developer curriculum to simplify onboarding. This includes Aiken for smart contracts, Mesh (or potentially a popular client SDK) for the frontend/off-chain, and Yaci DevKit for local development.
* **Target Audience Focus:** It was decided that the upcoming curriculum should focus on professional developer teams (e.g., those porting from other networks) rather than just casual hackathon participants.
* **Developer Portal Workflow:** It was confirmed that the "Developer Portal" remains the canonical source of truth. Contributors must fork the repository and submit PRs to a staging branch for weekly review before moving to production.
* **Entry Point Philosophy:** The group decided that while they will recommend a default toolset (Aiken/Mesh), they will aim to keep the high-level conceptual explanations "tooling agnostic" so as not to alienate developers using other languages like Python.

**Actions**

* Bora: Finalize the theoretical "crash course" curriculum (estimated at 8–9 hours) and share it with the DevX working group for review before proposing it formally within the Cardano Foundation.
* Bora: Create a project board (or issues) on the Developer Portal to track the technical tasks discussed, such as the sandbox environment and CLI tools.
* Bora: Work on a "Dev Container" or template repository (likely using Yaci and Mesh) that allows users to spin up a Cardano development environment with one click via GitHub Codespaces.
* Robertino: Continue refining the open-source strategy for a cardano-init CLI tool that scaffolds projects based on user preferences.
* **Robertino:** Investigate the feasibility of a "Can I Use" style status page for Cardano tooling to track feature parity across different SDKs.
* **Terence:** Coordinate with the Developer Advocates to ensure the DevX working group plans for Q2 are aligned with the new curriculum and portal updates.
* **Dan:** Update the "Developer Pathway" PR on the Developer Portal once the curriculum structure is finalized so the diagram can be accurately linked.

| Topic                      | Discussion                                                                                                                                                    | Notes                                                                                            |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| Builder Fest Locations     | The group discussed rumors regarding the next Builder Fest location, specifically mentioning Japan and Africa as potential candidates.                        | Robertino noted Africa’s high potential due to a hungry, young developer population.             |
| Africa Developer Potential | Robertino shared experiences teaching in Kenya; Bora emphasized targeting the region with ads for upcoming hackathons due to high crypto awareness.           | Focus on regions where users face high peer-to-payment friction.                                 |
| CF Developer Pipeline      | Bora is defining a full pipeline at the Cardano Foundation (CF) to move developers from hackathons to the Cardano Accelerator program.                        | Goal: Provide business services, financial counsel, and VC connections.                          |
| Onboarding Curriculum      | Bora is developing a "crash course" curriculum (8-9 hours) to reduce professional onboarding time from weeks to days.                                         | Designed for professional teams rather than casual hobbyists.                                    |
| Developer Portal PRs       | Dan and Bora discussed a pending Pull Request (PR) for a "Developer Pathway" mermaid diagram on the landing page.                                             | PR is on hold until the curriculum is ready to be linked to the pathway.                         |
| Staging Workflow           | Bora explained the standard workflow: contributors should fork the repo, submit PRs to staging, and updates move to production weekly.                        | Recommended using screenshots for quick feedback before formal staging.                          |
| DevX Working Group Q2      | Terence suggested aligning the developer advocates' efforts with Bora’s coursework to avoid duplicated work in Q2.                                            | Focus on "look and feel" consistency across different programs.                                  |
| Standardized Tech Stack    | Bora proposed a recommended (opinionated) stack: Aiken (on-chain), Mesh/Lucid (off-chain), and Yaci DevKit (local testing).                                   | Standardization is intended to simplify the entry point for newcomers.                           |
| Online Playgrounds         | Discussion on using GitHub Workspaces, Gitpod, or Demeter to provide one-click developer environments without local installation.                             | Demeter is reportedly winding down some services, making it a risky dependency.                  |
| The "Remix" Comparison     | Bernard highlighted the success of Ethereum’s Remix IDE, noting that Cardano lacks a similarly easy, browser-based "plug and play" tool.                      | Cardano’s architecture (EUTXO) makes browser-based node interaction more complex.                |
| Tooling Agnosticism        | Robertino and Bernard argued for respecting developer choice (Python, etc.), while Bora pushed for a "pragmatic" default to ensure things actually get built. | A compromise was suggested: a default "Aiken/Mesh" path with options to swap.                    |
| Maintenance & Resources    | Bora questioned who would actually build and maintain these tools (e.g., a CLI or Playground) as the current group lacks a dedicated engineering team.        | Developer Advocates (Emmanuel/Harun) currently handle technical tasks but have limited mandates. |
| Incentive Alignment        | Robertino suggested a "Can I Use" style site for Cardano tools to show which features work across different SDKs.                                             | This would incentivize SDK maintainers to fix "red" (broken) features to stay competitive.       |
| CLI Scaffolding            | Robertino plans to build a cardano-init CLI tool to scaffold projects based on user-selected languages if funding is secured.                                 | Aiming for a "one command" setup to lower the barrier to entry.                                  |
