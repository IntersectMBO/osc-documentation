# Documentation

## Documents found in Intersect Open Source Repos

A project must contain the following documents:

* `README`
* `DESCRIPTION`
* `LICENSE`
* `CONTRIBUTING.md`
* `CODE_OF_CONDUCT`
* `CODEOWNERS.md`
* A `CHANGELOG` (if the project includes multiple packages or similar, then one `CHANGELOG` per package may be more appropriate)
* `SECURITY.md` (this is currently being drafted by the Security TWG and will be pushed to all developers when ready.

## Other Items found in Intersect Open Source Repos

A project should contain the following documents:

* `RISSUE TEMPLATE`
* `PULL REQUEST (PR) TEMPLATE`

The documents should be easily accessible and discoverable, ideally by being put in standard locations.

The content of these documents is largely up to the project contributors, but we include some additional policies below In the following, when we say that a document should include information, this can either mean it includes it directly, or that it clearly links to where it can be found.

### README

A comprehensive overview of the project. It typically includes the project's purpose, installation instructions, usage examples, and any other important information a user or contributor needs to get started. The project `README` should include any information that is necessary according to the [governance policy](governance.md).

### DESCRIPTION

Often found in projects with specific language ecosystems (e.g., R packages), this file provides metadata about the project, such as its name, version, author, and dependencies.

### LICENSE

This file contains the full text of the license under which the project is distributed, specifying the terms and conditions for using, modifying, and distributing the software.

### CONTRIBUTING.md

A guide for contributors that outlines the process for contributing to the project. It typically includes guidelines on submitting issues and pull requests, coding standards, and any other relevant contribution protocols.

### CODE OF CONDUCT

A document that sets expectations for behavior within the project community to ensure a welcoming and respectful environment. It includes standards for behavior, reporting guidelines, and enforcement policies.

Individual projects SHOULD use the [default Code of Conduct in this repository](https://github.com/IntersectMBO/OSC-documentation/commit/224dd0eb4edfc9a44a4a618ceeb22cadc885655c), either by copying it or creating a `CODE_OF_CONDUCT` document that just links to it.

### CODEOWNERS

A file that specifies individuals or teams responsible for specific parts of the codebase. It helps streamline the code review and approval process by automatically assigning reviewers to pull requests.

### CHANGELOG.md

A log or record of all notable changes made to the project, usually organized by version number and release date. It includes lists of added features, bug fixes, and other changes. For ease of access there should be a `CHANGELOG` at the top-level of code. For larger projects there may be individual logs, however they all major changes should be viewable or linked in the top-level `CHANGELOG`.&#x20;

### SECURITY.md

A document that outlines the project's security policies, including how to report security vulnerabilities, response times, and guidelines for responsible disclosure.

### ISSUE TEMPLATE

A predefined template for reporting bugs or suggesting features. It helps standardize the information provided by users, making it easier for maintainers to understand and address issues.

### PULL REQUEST (PR) TEMPLATE

A predefined template for submitting pull requests. It guides contributors on how to structure their pull requests, often including a checklist to ensure all necessary information and steps are included.
