---
description: >-
  This is a bug bounty program focused around the Core Node, Intersect owned or
  sponsored prejcts.
---

# 🫢 Bug Bounty Program

#### Executive Summary

The Bug Bounty Program is designed to enhance the security of the ecosystem by incentivizing ethical hackers and security researchers to identify and responsibly disclose vulnerabilities. With a $300,000 budget for year 1, the program provides structured rewards based on severity and impact, ensuring proactive security measures while maintaining transparency and accountability.

The program operates under a three-tier governance model:

* Security Council – Handles incident management, vulnerability validation, and remediation efforts.
* Open Source Committee – Serves as a review-only body, providing oversight without execution authority, but validates the payment allocation.
* Open Source Office – Manages program execution, rewards distribution, and compliance.

#### Key Features of the Bug Bounty Program:

* Structured reward tiers: Payments range from $20,000 to $1,000 based on severity (Critical, High, Medium, Low).
* Clear reporting process: Researchers must provide detailed reports with proof of concept for validation.
* Responsible disclosure policy: Participants must follow strict guidelines to ensure ethical vulnerability reporting.
* Rapid response timelines: The Security Council will validate reports within 7-14 days and deploy fixes based on severity.
* Transparent reward distribution: Payments are processed within 30 days of validation, with multiple payout options (ADA, USDC, or fiat).
* Continuous improvement: Regular program audits, budget optimizations, and community engagement initiatives will ensure long-term success.

By implementing this structured and well-governed bug bounty program, the ecosystem strengthens its security resilience, fosters community participation, and upholds ethical vulnerability management practices.

### 1. Program Scope and Coverage

This section defines the boundaries of the bug bounty program, specifying which systems are eligible for testing and which activities are prohibited to ensure ethical participation.

#### 1.1 Systems and Assets in Scope

The bug bounty program applies to critical infrastructure and software components that are essential to the security and stability of the ecosystem.

**Eligible Targets:**

* Core Infrastructure – Systems directly supporting the network, including validator nodes and backend services.
* Smart Contracts & Blockchain Components – As applicable by SC review smart contract deployed on the blockchain.
* APIs & Web Applications – Public-facing APIs, developer tools, and user interfaces.
* Open-Source Repositories – Codebases managed by Intersect and other authorized repositories.

**Exclusions within In-Scope Assets:**

* Pre-release or beta features unless explicitly included in the program.
* Third-party dependencies unless otherwise specified.
* Assets that are part of controlled testing environments not yet deployed in production.

#### 1.2 Out-of-Scope Assets and Activities

To prevent abuse and ensure ethical participation, certain activities and targets are explicitly prohibited.

**Out-of-Scope Targets:**

* Social engineering attacks (e.g., phishing, impersonation, or blackmail).
* Denial of Service (DoS/DDoS) attacks that disrupt operations.
* Attacks on physical security infrastructure (e.g., hacking employee devices).
* Non-production environments unless explicitly authorized.
* Third-party services that are not directly managed by Intersect.

**Non-Qualifying Reports:**

* Publicly known issues (e.g., vulnerabilities already disclosed in security bulletins).
* Theoretical attacks without proof of exploitability.
* Bugs that require extensive user cooperation (e.g., social engineering-based exploits).

### 2.0 Vulnerability Classification and Reward Structure

This section defines how vulnerabilities are categorized, how reward amounts are determined, and how funds are managed to ensure the sustainability of the program.

#### 2.1 Classification Criteria (Critical, High, Medium, Low)

All reported vulnerabilities are categorized based on impact and exploitability, using the following severity levels:&#x20;

CVSS is utilized to measure impact scoring: [https://www.first.org/cvss/](https://www.first.org/cvss/)

| Severity Level | Description                                                                               | Example Scenarios                                                         |
| -------------- | ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| Critical       | Exploitable vulnerabilities that compromise funds, user data, or system control.          | Remote code execution, wallet private key leakage, full account takeover. |
| High           | Issues that lead to significant security breaches, requiring minimal user interaction.    | Authentication bypass, API abuse allowing unauthorized transactions.      |
| Medium         | Security flaws that require additional attack vectors to be exploited.                    | Information disclosure, improper access control, minor logic bugs.        |
| Low            | Issues that do not pose immediate security risks but could contribute to larger exploits. | Minor UI flaws affecting security, error messages revealing stack traces. |

#### 2.2 Reward Tiers and Payouts

Each severity level has a corresponding reward range, ensuring fair compensation based on impact. These ranges serve as a guidance and does wholly reflect an award, as each issue or big incident may justify a higher bounty depending on level of threat.

| Severity Level | Anticipated Reward Range |
| -------------- | ------------------------ |
| Critical       | $10,000 - $20,000        |
| High           | $5,000 - $10,000         |
| Medium         | $1,000 - $5,000          |
| Low            | Up to $1,000             |

**Factors Affecting Payout Amounts:**

* Quality of report: Clear documentation, proof of concept (PoC), and exploitability details.
* Reproducibility: Whether the vulnerability can be consistently replicated.
* Severity and impact: Higher impact vulnerabilities receive higher payouts.
* Novelty: Whether the vulnerability is previously unknown or a duplicate report.

#### 2.3 Reward Pool Distribution and Adjustments

To maintain the program’s longevity, funds are allocated strategically throughout the program duration.

**Budget Allocation Strategy:**

* $300,000 total pool for year 1, distributed based on reported vulnerabilities.
* Quarterly evaluations to assess program engagement and adjust payouts if needed.
* Emergency reserve allocation for handling high-impact security incidents.
* Roll-over funds policy – Unused funds can be shifted to subsequent program periods or returned to the treasury as overall budgetary policy dictates.

### 3.0 Reporting and Validation Process

This section outlines how security researchers should report vulnerabilities, the steps for validation, and the expected response times from the Security Council.

#### 3.1 Vulnerability Submission Guidelines

All vulnerability reports must be submitted through the GitHub private disclosure process ([https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/about-coordinated-disclosure-of-security-vulnerabilities?learn=security\_advisories\&learnproduct=code-security](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/about-coordinated-disclosure-of-security-vulnerabilities?learn=security_advisories\&learnproduct=code-security)), which ensures secure communication and proper tracking of submissions.

**Required Information for a Valid Submission:**

A report must include the following details:

1. Title – A concise name for the vulnerability.
2. Description – A clear explanation of the security issue and its impact.
3. Steps to Reproduce – A detailed, step-by-step guide demonstrating how to exploit the vulnerability.
4. Proof of Concept (PoC) – A working example showing exploitability (e.g., scripts, screenshots, or video walkthroughs).
5. Affected Component – Specify which system, smart contract, API, or software is vulnerable.
6. Suggested Remediation – If possible, provide recommendations on how to fix the issue.

**Submission Restrictions:**

* Reports must be original and unpublished at the time of submission.
* Researchers must not publicly disclose the vulnerability before the issue is patched.
* Automated scanning or brute-force techniques that degrade system performance are prohibited.

#### 3.2 Validation and Prioritization

Once a vulnerability is submitted, it goes through the Security Council’s validation process to confirm its authenticity and impact.

**Validation Steps:**

1. Acknowledgment – Initial confirmation of submission within 24 hours.
2. Triage and Reproduction – The Security Council attempts to reproduce the issue within 3-7 days, depending on complexity.
3. Severity Classification – The issue is categorized based on impact (Critical, High, Medium, Low).
4. Fix Deployment Planning – The Security Council coordinates with developers to determine a remediation timeline.
5. Researcher Notification – The submitter is informed of classification and next steps.

**Duplicate Reports Policy:**

* If multiple researchers submit the same vulnerability, only the first valid report will be rewarded.
* If a similar report adds significant new details, it may receive partial recognition.

#### 3.3 Communication and Response Times

To maintain transparency and efficiency, the following response timelines are enforced:

| Action                               | Response Time                                        |
| ------------------------------------ | ---------------------------------------------------- |
| Acknowledgment of submission         | Within 24 hours                                      |
| Validation & severity classification | Within 7-14 days                                     |
| Fix deployment timeline              | Critical: 7 days, High: 14 days, Medium/Low: 30 days |
| Final researcher notification        | Within 30 days of fix deployment                     |
| Reward payout processing             | Within 30 days of validation                         |

**Security Council Escalations:**

If a vulnerability presents an immediate, system-wide risk, the Security Council will escalate the issue immediately, bypassing standard timelines for an emergency response.

### 4.0 Governance and Oversight

The Bug Bounty Program operates under a structured governance model that ensures accountability, transparency, and efficient execution. The governance structure consists of three key entities:

1. Security Council – Handles all incident management and response activities.
2. Open Source Committee – A review-only body providing oversight without execution authority.
3. Open Source Office – Responsible for execution and administration of the program.

#### 4.1 Security Council: Roles and Responsibilities

The Security Council is the primary authority responsible for managing vulnerabilities reported through the bug bounty program.

**Key Responsibilities:**

* Triage and validate vulnerability reports received from security researchers.
* Categorize vulnerabilities based on severity and assign priorities.
* Coordinate remediation efforts with developers and security engineers.
* Ensure proper ethical reporting practices and enforce disclosure policies.
* Escalate major security incidents to the appropriate body depending on the issue raised. (Technical Steering Committee, Open Source Committee, or Security Council).
* Provide quarterly reports on program performance, trends, and challenges.

**Composition:**

* Security Engineers
* Incident Response Specialists
* Threat Analysts
* External Security Experts (if applicable)

#### 4.2 Open Source Committee: Review and Oversight

The Open Source Committee acts as an oversight body ensuring the program aligns with the broader open-source security goals. However, it does not have direct execution authority.

**Key Responsibilities:**

* Review program policies and governance structures to ensure alignment with community values.
* Audit budget utilization and make recommendations for adjustments if necessary.
* Evaluate the effectiveness of the Security Council’s decisions.
* Approve high-level policy changes while leaving execution to the Open Source Office.
* Act as an advisory body in security escalations and incident reviews.

**Limitations:**

* Does not handle day-to-day program execution.
* Cannot directly distribute rewards or approve specific reports.

#### 4.3 Open Source Office: Execution and Administration

The Open Source Office is responsible for executing the Bug Bounty Program by handling day-to-day operations, payments, and communication.

**Key Responsibilities:**

* Process rewards and payments for validated reports.
* Manage community engagement and respond to inquiries from security researchers.
* Ensure legal and compliance adherence related to the program.
* Handle public reporting and transparency efforts (e.g., publishing reports on vulnerabilities and resolutions).
* Coordinate with the Security Council to ensure proper funding and resource allocation.

**Execution Power:**

The Open Source Office has full operational control over the program’s implementation, ensuring that all validated vulnerabilities are addressed efficiently and transparently.

\
