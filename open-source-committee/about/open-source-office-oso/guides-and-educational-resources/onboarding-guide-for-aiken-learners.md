---
description: >-
  This page is in active construction and welcome to feedback for any
  inaccuracies.
---

# 😉 Onboarding Guide for Aiken Learners

## 📘 Aiken Smart Contract Learning Resources (All Levels)

Aiken is a modern, strictly-typed smart contract language built for the Cardano blockchain. Inspired by Elm and Rust, it was designed to be fast, safe, and developer-friendly. Unlike Plutus, Aiken compiles directly to Plutus Core without requiring Haskell expertise, making it ideal for developers entering the Cardano smart contract ecosystem.

Below, resources are organized into books (docs), tutorials, video walkthroughs, interactive platforms, and Cardano-specific deployment tools. A detailed learning path is included at the end to guide you from zero to full-stack smart contract development.

***

### 📘 Documentation & Language References

**Aiken Official Documentation** – Free/All Levels\
https://aiken-lang.org/docs\
The central resource for everything Aiken. Includes installation instructions, syntax explanations, a full language tour, blueprint format spec, and deployment examples.

**Language Tour** – Free/Beginner\
https://aiken-lang.org/docs/reference/language-tour\
Covers Aiken syntax, functions, types, modules, and pattern matching.

**Blueprint Format** – Free/Intermediate\
https://aiken-lang.org/docs/reference/blueprints\
Explains how Aiken packages smart contracts into deployable blueprints with validator definitions and metadata.

**GitHub Source Repositories** – Free/All Levels

* Compiler: [https://github.com/aiken-lang/aiken](https://github.com/aiken-lang/aiken)
* Standard Library: [https://github.com/aiken-lang/stdlib](https://github.com/aiken-lang/stdlib)
* Examples: [https://github.com/aiken-lang/examples](https://github.com/aiken-lang/examples)
* Playground (in development): [https://github.com/aiken-lang/playground](https://github.com/aiken-lang/playground)

***

### 📚 Tutorials & Example Projects

**Hello World Tutorial** – Free/Beginner\
https://aiken-lang.org/docs/tutorials/hello-world\
A full walk-through of building, testing, and simulating a UTxO validator in Aiken. Ideal for first-time smart contract developers.

**Vesting Contract** – Free/Intermediate\
https://aiken-lang.org/docs/examples/vesting\
A contract that unlocks ADA after a set time. Includes off-chain interaction via Mesh.

**Gift Card Validator** – Free/Intermediate\
[https://github.com/aiken-lang/awesome-aiken#examples](https://github.com/aiken-lang/awesome-aiken#examples)\
An example dApp with redeemable NFTs, showing validator logic and blueprint structure.

**Full-stack dApp with MeshJS** – Free/Intermediate–Advanced\
https://meshjs.dev/guides/smart-contracts\
How to deploy Aiken contracts in a real frontend using Mesh and Cardano testnet.

**Escrow, Royalty, and Swap Contracts** – Free/Advanced\
https://meshjs.dev/libraries/smart-contract\
Mesh contract templates written in Aiken. Ready to customize for production use.

***

### 🎥 Video Courses & Walkthroughs

**StoicPool Aiken Video Series (Rhys Morgan)** – Free/Beginner–Intermediate\
[https://www.youtube.com/@stoicpool](https://www.youtube.com/@stoicpool)\
An 8-part YouTube series from a Cardano SPO. Covers project setup, validator logic, and off-chain interaction.

**ReddSpark Beginner Walkthrough** – Free/Beginner\
[https://www.youtube.com/watch?v=N-JmswJuQRU](https://www.youtube.com/watch?v=N-JmswJuQRU)\
Windows-based walkthrough showing the Hello World flow with commentary and troubleshooting tips.

**Cardano Foundation Hackathon Sessions** – Free/Intermediate\
Includes practical contract demos and advanced validator concepts presented during Cardano Summit workshops.

**MeshJS + Aiken Walkthroughs** – Free/Intermediate\
Visual step-throughs on YouTube and Mesh docs showing how to test and deploy Aiken validators in a web frontend.

***

### 💻 Interactive Platforms & Development Tools

**Aikup Installer (for CLI)** – Free\
https://aikup.dev/install\
Cross-platform CLI installer for Aiken. Automatically sets up your environment.

**Aiken CLI** – Free\
Includes:

* `aiken check` – Type/syntax check
* `aiken test` – Unit/property tests
* `aiken build` – Plutus Core compilation
* `aiken blueprint` – Deployment packaging\
  Docs

**VS Code Extension** – Free\
[https://marketplace.visualstudio.com/items?itemName=aiken-lang.aiken](https://marketplace.visualstudio.com/items?itemName=aiken-lang.aiken)\
Offers syntax highlighting, inline errors, and autocomplete for Aiken projects.

**Playground (In Development)**\
[https://github.com/aiken-lang/playground](https://github.com/aiken-lang/playground)\
A browser-based Aiken environment to simulate validators without installing anything locally.

***

### 🧑‍🏫 Structured Learning Tracks

**Plutus PBL Curriculum (w/ Aiken Modules)** – Free\
[https://plutuspbl.io](https://plutuspbl.io)\
A project-based curriculum featuring Aiken validator labs and smart contract challenges.

**Catalyst-Funded Aiken Education Projects** – Free (if funded)\
Look for funded proposals like:

* “Aiken Alive”
* “Aiken Bootcamp Vietnam”\
  These offer free, structured education delivered by the community. Check updates at [Project Catalyst](https://projectcatalyst.io).

***

### 🌐 Community Resources & Support

**Awesome Aiken (Community Curated)** – Free\
[https://github.com/aiken-lang/awesome-aiken](https://github.com/aiken-lang/awesome-aiken)\
A curated repository of templates, tools, tutorials, validator logic, and dApp demos.

**Aiken GitHub Organization** – Free\
[https://github.com/aiken-lang](https://github.com/aiken-lang)\
Home of the Aiken compiler, stdlib, and example projects.

**Discord: Cardano Devs #aiken-lang** – Free\
https://discord.gg/cardano\
Aiken support is active under the #aiken-lang channel. Includes core contributors and friendly SPOs.

**Cardano Stack Exchange**\
[https://cardano.stackexchange.com](https://cardano.stackexchange.com)\
Q\&A for developer-specific issues using Aiken in the EUTXO model.

**Reddit Discussions**\
[https://reddit.com/r/cardano](https://reddit.com/r/cardano)\
Real-world Aiken projects, problems, and community learning journeys are often shared here.

***

### 🧭 Suggested Learning Path

| Phase                 | Focus Area                           | Recommended Resources                        |
| --------------------- | ------------------------------------ | -------------------------------------------- |
| 🟢 Getting Started    | Install Aiken + Write First Contract | Aikup, Hello World, Language Tour            |
| 🟡 Build Projects     | Write Real Validators, Test Logic    | Vesting + Gift Card, Blueprint docs          |
| 🔵 Full Stack Dev     | Off-chain + UI integration           | MeshJS Walkthroughs, Lucid, PyCardano        |
| 🟣 Power User         | Reusable Contracts, Testing, CI      | Mesh Libraries, `aiken test`, GitHub Actions |
| 🟠 Community Learning | Join Groups, Get Help, Contribute    | Discord, Awesome-Aiken, Catalyst Proposals   |
